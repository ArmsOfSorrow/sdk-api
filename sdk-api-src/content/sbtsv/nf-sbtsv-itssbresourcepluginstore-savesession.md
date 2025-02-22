---
UID: NF:sbtsv.ITsSbResourcePluginStore.SaveSession
title: ITsSbResourcePluginStore::SaveSession (sbtsv.h)
description: Saves a session.
old-location: termserv\itssbresourcepluginstore_savesession.htm
tech.root: TermServ
ms.assetid: a4f29a99-8478-425d-91d7-c771c35bb2fa
ms.date: 12/05/2018
ms.keywords: ITsSbResourcePluginStore interface [Remote Desktop Services],SaveSession method, ITsSbResourcePluginStore.SaveSession, ITsSbResourcePluginStore::SaveSession, ITsSbResourcePluginStoreEx interface [Remote Desktop Services],SaveSession method, ITsSbResourcePluginStoreEx::SaveSession, SaveSession, SaveSession method [Remote Desktop Services], SaveSession method [Remote Desktop Services],ITsSbResourcePluginStore interface, SaveSession method [Remote Desktop Services],ITsSbResourcePluginStoreEx interface, sbtsv/ITsSbResourcePluginStore::SaveSession, sbtsv/ITsSbResourcePluginStoreEx::SaveSession, termserv.itssbresourcepluginstore_savesession
ms.topic: method
f1_keywords:
- sbtsv/ITsSbResourcePluginStore.SaveSession
dev_langs:
- c++
req.header: sbtsv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Sbtsv.idl
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
- sbtsv.h
api_name:
- ITsSbResourcePluginStore.SaveSession
- ITsSbResourcePluginStoreEx.SaveSession
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITsSbResourcePluginStore::SaveSession


## -description


Saves a session.


## -parameters




### -param pSession [in]

A Pointer to the <a href="https://docs.microsoft.com/windows/desktop/api/sbtsv/nn-sbtsv-itssbsession">ITsSbSession</a> object to save.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/sbtsv/nn-sbtsv-itssbresourcepluginstore">ITsSbResourcePluginStore</a>



<a href="https://docs.microsoft.com/windows/desktop/TermServ/itssbresourcepluginstoreex">ITsSbResourcePluginStoreEx</a>
 

 

