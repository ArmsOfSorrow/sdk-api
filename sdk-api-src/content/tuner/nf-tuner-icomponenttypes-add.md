---
UID: NF:tuner.IComponentTypes.Add
title: IComponentTypes::Add (tuner.h)
description: The Add method adds a new ComponentType object to the collection.
old-location: mstv\icomponenttypes_add.htm
tech.root: mstv
ms.assetid: 157f8d81-dbbf-44a7-9786-0758d3c89634
ms.date: 12/05/2018
ms.keywords: Add, Add method [Microsoft TV Technologies], Add method [Microsoft TV Technologies],IComponentTypes interface, IComponentTypes interface [Microsoft TV Technologies],Add method, IComponentTypes.Add, IComponentTypes::Add, IComponentTypesAdd, mstv.icomponenttypes_add, tuner/IComponentTypes::Add
ms.topic: method
f1_keywords:
- tuner/IComponentTypes.Add
dev_langs:
- c++
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
- tuner.h
api_name:
- IComponentTypes.Add
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IComponentTypes::Add


## -description



The <b>Add</b> method adds a new <a href="https://docs.microsoft.com/previous-versions/windows/desktop/legacy/dd693036(v=vs.85)">ComponentType</a> object to the collection.




## -parameters




### -param ComponentType [in]

Pointer to the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tuner/nn-tuner-icomponenttype">IComponentType</a> object that will be added to the collection.


### -param NewIndex [out]

The index number of the component type after it has been added to the collection.


## -returns



Returns S_OK if successful. If the method fails, error information can be retrieved using the standard COM <b>IErrorInfo</b> interface.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tuner/nn-tuner-icomponenttypes">IComponentTypes Interface</a>
 

 

