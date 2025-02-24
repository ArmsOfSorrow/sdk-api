---
UID: NF:wbemcli.IWbemContext.DeleteValue
title: IWbemContext::DeleteValue (wbemcli.h)
description: The IWbemContext::DeleteValue method deletes a named context value created by IWbemContext::SetValue.
old-location: wmi\iwbemcontext_deletevalue.htm
tech.root: WmiSdk
ms.assetid: 5f2956cf-8901-441f-b1bd-4b2f21d74683
ms.date: 12/05/2018
ms.keywords: DeleteValue, DeleteValue method [Windows Management Instrumentation], DeleteValue method [Windows Management Instrumentation],IWbemContext interface, IWbemContext interface [Windows Management Instrumentation],DeleteValue method, IWbemContext.DeleteValue, IWbemContext::DeleteValue, _hmm_iwbemcontext_deletevalue, wbemcli/IWbemContext::DeleteValue, wmi.iwbemcontext_deletevalue
ms.topic: method
f1_keywords:
- wbemcli/IWbemContext.DeleteValue
dev_langs:
- c++
req.header: wbemcli.h
req.include-header: Wbemidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wbemuuid.lib
req.dll: Esscli.dll; Fastprox.dll; FrameDyn.dll; FrameDynOS.dll; Wbemcomn.dll; Wbemcore.dll; Wbemess.dll; Wmipjobj.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Esscli.dll
- Fastprox.dll
- FrameDyn.dll
- FrameDynOS.dll
- Wbemcomn.dll
- Wbemcore.dll
- Wbemess.dll
- Wmipjobj.dll
api_name:
- IWbemContext.DeleteValue
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWbemContext::DeleteValue


## -description


The 
<b>IWbemContext::DeleteValue</b> method deletes a named context value created by 
<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemcontext-setvalue">IWbemContext::SetValue</a>.


## -parameters




### -param wszName [in]

Pointer to a valid <b>BSTR</b> containing the named context value to delete. The pointer is treated as read-only.


### -param lFlags [in]

Reserved. This parameter must be 0.


## -returns



This method returns an <b>HRESULT</b>HRESULT indicating the status of the method call. The following list lists the value contained withinan <b>HRESULT</b>HRESULT.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nn-wbemcli-iwbemcontext">IWbemContext</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemcontext-getvalue">IWbemContext::GetValue</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemcontext-setvalue">IWbemContext::SetValue</a>
 

 

