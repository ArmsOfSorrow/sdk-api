---
UID: NF:bdaiface.IBDA_FrequencyFilter.get_Bandwidth
title: IBDA_FrequencyFilter::get_Bandwidth (bdaiface.h)
description: The get_Bandwidth method retrieves the bandwidth.
old-location: mstv\ibda_frequencyfilter_get_bandwidth.htm
tech.root: mstv
ms.assetid: 3cea7bbe-488b-4c5c-84a8-28f0dc77e3c1
ms.date: 12/05/2018
ms.keywords: IBDA_FrequencyFilter interface [Microsoft TV Technologies],get_Bandwidth method, IBDA_FrequencyFilter.get_Bandwidth, IBDA_FrequencyFilter::get_Bandwidth, IBDA_FrequencyFilterget_Bandwidth, bdaiface/IBDA_FrequencyFilter::get_Bandwidth, get_Bandwidth, get_Bandwidth method [Microsoft TV Technologies], get_Bandwidth method [Microsoft TV Technologies],IBDA_FrequencyFilter interface, mstv.ibda_frequencyfilter_get_bandwidth
ms.topic: method
f1_keywords:
- bdaiface/IBDA_FrequencyFilter.get_Bandwidth
dev_langs:
- c++
req.header: bdaiface.h
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
- COM
api_location:
- bdaiface.h
api_name:
- IBDA_FrequencyFilter.get_Bandwidth
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IBDA_FrequencyFilter::get_Bandwidth


## -description



The <b>get_Bandwidth</b> method retrieves the bandwidth.




## -parameters




### -param pulBandwidth [out]

Pointer that receives the bandwidth. The units are 1 Hz x the frequency multiplier, where the <i>frequency multiplier</i> is the value returned by the <a href="https://docs.microsoft.com/windows/desktop/api/bdaiface/nf-bdaiface-ibda_frequencyfilter-get_frequencymultiplier">IBDA_FrequencyFilter::get_FrequencyMultiplier</a> method. The default frequency multiplier is 1000, so the default units are kilohertz (kHz).


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/error-and-success-codes">Error and Success Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/bdaiface/nn-bdaiface-ibda_frequencyfilter">IBDA_FrequencyFilter Interface</a>



<a href="https://docs.microsoft.com/windows/desktop/api/bdaiface/nf-bdaiface-ibda_frequencyfilter-put_bandwidth">IBDA_FrequencyFilter::put_Bandwidth</a>
 

 

