---
UID: NF:oleauto.VarBoolFromUI8
title: VarBoolFromUI8 function (oleauto.h)
description: Converts an 8-byte unsigned integer value to a Boolean value.
old-location: automat\varboolfromui8.htm
tech.root: automat
ms.assetid: 4a5861b0-cc39-46de-ae39-f34a179bb9d0
ms.date: 12/05/2018
ms.keywords: VarBoolFromUI8, VarBoolFromUI8 function [Automation], _oa96_VarBoolFromUI8, automat.varboolfromui8, oleauto/VarBoolFromUI8
ms.topic: function
f1_keywords:
- oleauto/VarBoolFromUI8
dev_langs:
- c++
req.header: oleauto.h
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
req.lib: OleAut32.lib
req.dll: OleAut32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- OleAut32.dll
api_name:
- VarBoolFromUI8
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# VarBoolFromUI8 function


## -description


Converts an 8-byte unsigned integer value to a Boolean value.


## -parameters




### -param i64In [in]

The value to convert.


### -param pboolOut [out]

The resulting value.


## -returns



This function can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DISP_E_BADVARTYPE</b></dt>
</dl>
</td>
<td width="60%">
The input parameter is not a valid type of variant.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DISP_E_OVERFLOW</b></dt>
</dl>
</td>
<td width="60%">
The data pointed to by the output parameter does not fit in the destination type.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DISP_E_TYPEMISMATCH</b></dt>
</dl>
</td>
<td width="60%">
The argument could not be coerced to the specified type.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One of the arguments is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory to complete the operation.

</td>
</tr>
</table>
 



