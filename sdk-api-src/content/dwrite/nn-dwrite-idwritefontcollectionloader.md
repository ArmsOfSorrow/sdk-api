---
UID: NN:dwrite.IDWriteFontCollectionLoader
title: IDWriteFontCollectionLoader (dwrite.h)
description: Used to construct a collection of fonts given a particular type of key.
old-location: directwrite\IDWriteFontCollectionLoader.htm
tech.root: DirectWrite
ms.assetid: 898645ce-4bd5-4491-a31c-f60a17578872
ms.date: 12/05/2018
ms.keywords: IDWriteFontCollectionLoader, IDWriteFontCollectionLoader interface [Direct Write], IDWriteFontCollectionLoader interface [Direct Write],described, directwrite.IDWriteFontCollectionLoader, dwrite/IDWriteFontCollectionLoader
ms.topic: interface
f1_keywords:
- dwrite/IDWriteFontCollectionLoader
dev_langs:
- c++
req.header: dwrite.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dwrite.lib
req.dll: Dwrite.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- dwrite.dll
api_name:
- IDWriteFontCollectionLoader
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDWriteFontCollectionLoader interface


## -description


  Used to construct a collection of fonts given a particular type of key. 


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDWriteFontCollectionLoader</b> interface inherits from the <a href="/windows/win32/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IDWriteFontCollectionLoader</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDWriteFontCollectionLoader</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="/windows/win32/api/dwrite/nf-dwrite-idwritefontcollectionloader-createenumeratorfromkey">CreateEnumeratorFromKey</a>
</td>
<td align="left" width="63%">
 Creates a font file enumerator object that encapsulates a collection of font files.
     The font system calls back to this interface to create a font collection.

</td>
</tr>
</table> 


## -remarks



The font collection loader interface is recommended to be implemented by a singleton object. Note that font collection loader implementations must not register themselves with DirectWrite factory inside their constructors and must not unregister themselves in their destructors, because registration and unregistraton operations increment and decrement the object reference count respectively. Instead, registration and unregistration of font file loaders with DirectWrite factory should be performed outside of the font file loader implementation as a separate step.



