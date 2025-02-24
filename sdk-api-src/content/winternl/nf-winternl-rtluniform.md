---
UID: NF:winternl.RtlUniform
title: RtlUniform function (winternl.h)
description: Generates a uniform random number using D.H. Lehmer's 1948 algorithm.
old-location: winprog\rtluniform.htm
tech.root: DevNotes
ms.assetid: 78bb05fa-3ebc-4e61-ae4f-58544da51200
ms.date: 12/05/2018
ms.keywords: RtlUniform, RtlUniform function [Windows API], winprog.rtluniform, winternl/RtlUniform
ms.topic: function
f1_keywords:
- winternl/RtlUniform
dev_langs:
- c++
req.header: winternl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
req.dll: Ntdll.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Ntdll.dll
api_name:
- RtlUniform
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# RtlUniform function


## -description


Generates a uniform random number using D.H. Lehmer's 1948 algorithm.


## -parameters




### -param Seed [in, out]

The seed value.


## -returns



 The function returns a random number uniformly distributed over [0..MAXLONG].




## -remarks



This function has no associated import library. You must use the <a href="https://docs.microsoft.com/windows/desktop/api/libloaderapi/nf-libloaderapi-loadlibrarya">LoadLibrary</a> and <a href="https://docs.microsoft.com/windows/desktop/api/libloaderapi/nf-libloaderapi-getprocaddress">GetProcAddress</a> functions to dynamically link to Ntdll.dll.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wincrypt/nf-wincrypt-cryptgenrandom">CryptGenRandom</a>
 

 

