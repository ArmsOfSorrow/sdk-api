---
UID: NF:faxcomex.IFaxOutboundRoutingRule.Refresh
title: IFaxOutboundRoutingRule::Refresh (faxcomex.h)
description: The IFaxOutboundRoutingRule::Refresh method refreshes FaxOutboundRoutingRule object information from the fax server.
old-location: fax\_mfax_faxoutboundroutingrule_cpp_mfax_faxoutboundroutingrule_refresh_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_6s2w.htm
ms.date: 12/05/2018
ms.keywords: IFaxOutboundRoutingRule interface [Fax Service],Refresh method, IFaxOutboundRoutingRule.Refresh, IFaxOutboundRoutingRule::Refresh, Refresh, Refresh method [Fax Service], Refresh method [Fax Service],IFaxOutboundRoutingRule interface, _mfax_faxoutboundroutingrule.refresh, fax._mfax_faxoutboundroutingrule_cpp_mfax_faxoutboundroutingrule_refresh_cpp, fax._mfax_faxoutboundroutingrule_refresh, faxcomex/IFaxOutboundRoutingRule::Refresh
ms.topic: method
f1_keywords:
- faxcomex/IFaxOutboundRoutingRule.Refresh
dev_langs:
- c++
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Fxscomex.dll
api_name:
- IFaxOutboundRoutingRule.Refresh
- IFaxOutboundRoutingRule.Refresh
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFaxOutboundRoutingRule::Refresh


## -description


The <b>IFaxOutboundRoutingRule::Refresh</b> method refreshes <a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-faxoutboundroutingrule">FaxOutboundRoutingRule</a> object information from the fax server.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



When the <b>IFaxOutboundRoutingRule::Refresh</b> method is called, any configuration changes made after the last <a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-faxoutboundroutingrule-save-vb">IFaxOutboundRoutingRule::Save</a> method call are lost.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-faxoutboundroutingrule">FaxOutboundRoutingRule</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/faxcomex/nn-faxcomex-ifaxoutboundroutingrule">IFaxOutboundRoutingRule</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-creating-and-managing-outbound-routing-rules">Visual Basic Example</a>
 

 

