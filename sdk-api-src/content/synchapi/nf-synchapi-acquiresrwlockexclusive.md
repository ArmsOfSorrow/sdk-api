---
UID: NF:synchapi.AcquireSRWLockExclusive
title: AcquireSRWLockExclusive function (synchapi.h)
description: Acquires a slim reader/writer (SRW) lock in exclusive mode.
old-location: base\acquiresrwlockexclusive.htm
tech.root: Sync
ms.assetid: 02e987a2-4c2f-4ccb-8816-c04320b568c1
ms.date: 12/05/2018
ms.keywords: AcquireSRWLockExclusive, AcquireSRWLockExclusive function, base.acquiresrwlockexclusive, synchapi/AcquireSRWLockExclusive, winbase/AcquireSRWLockExclusive
ms.topic: function
f1_keywords:
- synchapi/AcquireSRWLockExclusive
dev_langs:
- c++
req.header: synchapi.h
req.include-header: Windows 7, Windows Server 2008  Windows Server 2008 R2, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Kernel32.dll
- API-MS-Win-Core-Synch-l1-1-0.dll
- KernelBase.dll
- API-MS-Win-Core-Synch-l1-2-0.dll
- API-MS-Win-Core-Synch-l1-2-1.dll
- API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
- MinKernelBase.dll
- vertdll.dll
api_name:
- AcquireSRWLockExclusive
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# AcquireSRWLockExclusive function


## -description


Acquires a slim reader/writer (SRW) lock in exclusive mode.


## -parameters




### -param SRWLock [in, out]

A pointer to the SRW lock.


## -returns



This function does not return a value.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/synchapi/nf-synchapi-releasesrwlockexclusive">ReleaseSRWLockExclusive</a>



<a href="https://docs.microsoft.com/windows/desktop/Sync/slim-reader-writer--srw--locks">Slim Reader/Writer (SRW) Locks</a>



<a href="https://docs.microsoft.com/windows/desktop/Sync/synchronization-functions">Synchronization Functions</a>
 

 

