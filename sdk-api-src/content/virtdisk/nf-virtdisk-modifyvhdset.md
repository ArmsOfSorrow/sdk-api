---
UID: NF:virtdisk.ModifyVhdSet
title: ModifyVhdSet function (virtdisk.h)
description: Modifies the internal contents of a virtual disk file. Can be used to set the active leaf, or to fix up snapshot entries.
old-location: vhd\modifyvhdset.htm
tech.root: VStor
ms.assetid: C0BDAF45-8F87-4EF5-81F3-F15E7E575EA1
ms.date: 12/05/2018
ms.keywords: ModifyVhdSet, ModifyVhdSet function [VHD], vdssys/ModifyVhdSet, vhd.modifyvhdset, virtdisk/ModifyVhdSet
ms.topic: function
f1_keywords:
- virtdisk/ModifyVhdSet
dev_langs:
- c++
req.header: virtdisk.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: VirtDisk.lib
req.dll: VirtDisk.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- VirtDisk.dll
api_name:
- ModifyVhdSet
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ModifyVhdSet function


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Modifies the internal contents of a virtual disk file. Can be used to set the active leaf, or to fix up snapshot entries.


## -parameters




### -param VirtualDiskHandle [in]

A handle to the open virtual disk. This must be a VHD Set file.


### -param Parameters [in]

A pointer to a valid <a href="https://docs.microsoft.com/windows/win32/api/virtdisk/ns-virtdisk-modify_vhdset_parameters">MODIFY_VHDSET_PARAMETERS</a> structure that contains modification data.


### -param Flags [in]

Modification flags, which must be a valid combination of the <a href="https://docs.microsoft.com/windows/win32/api/virtdisk/ne-virtdisk-modify_vhdset_flag">MODIFY_VHDSET_FLAG</a> enumeration.


## -returns



Status of the request.

If the function succeeds, the return value is <b>ERROR_SUCCESS</b>.

If the function fails, the return value is an error code. For more information, see 
       <a href="https://docs.microsoft.com/windows/desktop/Debug/system-error-codes">System Error Codes</a>.



