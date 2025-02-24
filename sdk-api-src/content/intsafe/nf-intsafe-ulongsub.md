---
UID: NF:intsafe.ULongSub
title: ULongSub function (intsafe.h)
description: Subtracts one value of type ULONG from another.
old-location: shell\ULongSub.htm
tech.root: shell
ms.assetid: 5d2335a4-2b2e-4820-ae82-ba94d6e4cc9a
ms.date: 12/05/2018
ms.keywords: DWordSub, ULongSub, ULongSub function [Windows Shell], _shell_ULongSub, intsafe/ULongSub, shell.ULongSub
ms.topic: function
f1_keywords:
- intsafe/ULongSub
dev_langs:
- c++
req.header: intsafe.h
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
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- Intsafe.h
api_name:
- ULongSub
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ULongSub function


## -description


Subtracts one value of type <b>ULONG</b> from another.


## -parameters




### -param ulMinuend [in]

Type: <b>ULONG</b>

The value from which <i>ulSubtrahend</i> is subtracted.


### -param ulSubtrahend [in]

Type: <b>ULONG</b>

The value to subtract from <i>ulMinuend</i>.


### -param pulResult [out]

Type: <b>ULONG*</b>

A pointer to the result. If the operation results in a value that overflows or underflows the capacity of the type, the function returns INTSAFE_E_ARITHMETIC_OVERFLOW and this parameter is not valid.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This is one of a set of inline functions designed to provide arithmetic operations and perform validity checks with minimal impact on performance.

<b>DWordSub</b> is an alias for this function.



