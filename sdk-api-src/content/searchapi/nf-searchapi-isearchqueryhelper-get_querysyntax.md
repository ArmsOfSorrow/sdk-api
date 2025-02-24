---
UID: NF:searchapi.ISearchQueryHelper.get_QuerySyntax
title: ISearchQueryHelper::get_QuerySyntax (searchapi.h)
description: Gets the syntax of the query.
old-location: search\_search_ISearchQueryHelper_get_QuerySyntax.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\querying\isearchqueryhelper\get_querysyntax.htm
ms.date: 12/05/2018
ms.keywords: ISearchQueryHelper interface [search],get_QuerySyntax method, ISearchQueryHelper.get_QuerySyntax, ISearchQueryHelper::get_QuerySyntax, _search_ISearchQueryHelper_get_QuerySyntax, get_QuerySyntax, get_QuerySyntax method [search], get_QuerySyntax method [search],ISearchQueryHelper interface, search._search_ISearchQueryHelper_get_QuerySyntax, searchapi/ISearchQueryHelper::get_QuerySyntax
ms.topic: method
f1_keywords:
- searchapi/ISearchQueryHelper.get_QuerySyntax
dev_langs:
- c++
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Searchapi.h
api_name:
- ISearchQueryHelper.get_QuerySyntax
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
ms.custom: 19H1
---

# ISearchQueryHelper::get_QuerySyntax


## -description


Gets the syntax of the query.


## -parameters




### -param pQuerySyntax [out, retval]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/searchapi/ne-searchapi-search_query_syntax">SEARCH_QUERY_SYNTAX</a>*</b>

Receives a pointer to a value from the <a href="https://docs.microsoft.com/windows/desktop/api/searchapi/ne-searchapi-search_query_syntax">SEARCH_QUERY_SYNTAX</a> enumeration. 


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The allowed syntaxes are Simple, Natural Query Syntax (NQS), and Advanced Query Syntax (AQS). If not set, the default query syntax is SEARCH_ADVANCED_QUERY_SYNTAX.

The DSearch code sample, available on <a href="http://go.microsoft.com/fwlink/p/?linkid=155654">Code Gallery</a> and the <a href="http://go.microsoft.com/fwlink/p/?linkid=129787">Windows 7 SDK</a>, demonstrates how to create a class for a static console application to query Windows Search using the Microsoft.Search.Interop assembly for <a href="https://docs.microsoft.com/windows/desktop/api/searchapi/nn-searchapi-isearchqueryhelper">ISearchQueryHelper</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/searchapi/nn-searchapi-isearchqueryhelper">ISearchQueryHelper</a>



<a href="https://docs.microsoft.com/windows/desktop/api/searchapi/nf-searchapi-isearchqueryhelper-put_querysyntax">ISearchQueryHelper::put_QuerySyntax</a>



<a href="https://docs.microsoft.com/windows/desktop/search/-search-3x-wds-qryidx-overview">Querying the Index Programmatically</a>



<a href="https://docs.microsoft.com/windows/desktop/search/-search-sql-windowssearch-entry">Querying the Index with Windows Search SQL Syntax</a>
 

 

