---
UID: NN:d3d10_1.ID3D10BlendState1
title: ID3D10BlendState1 (d3d10_1.h)
description: This blend-state interface accesses blending state for a Direct3D 10.1 device for the output-merger stage.
old-location: direct3d10\id3d10blendstate1.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10blendstate1.htm
ms.date: 12/05/2018
ms.keywords: 50959f42-4209-b827-553e-862c94c85dfc, ID3D10BlendState1, ID3D10BlendState1 interface [Direct3D 10], ID3D10BlendState1 interface [Direct3D 10],described, d3d10_1/ID3D10BlendState1, direct3d10.id3d10blendstate1
ms.topic: interface
f1_keywords:
- d3d10_1/ID3D10BlendState1
dev_langs:
- c++
req.header: d3d10_1.h
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
req.lib: D3D10.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D3D10.lib
- D3D10.dll
api_name:
- ID3D10BlendState1
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10BlendState1 interface


## -description


This blend-state interface accesses blending state for a Direct3D 10.1 device for the <a href="https://docs.microsoft.com/windows/desktop/direct3d11/d3d10-graphics-programming-guide-output-merger-stage">output-merger</a> stage.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ID3D10BlendState1</b> interface inherits from <a href="https://docs.microsoft.com/windows/desktop/api/d3d10/nn-d3d10-id3d10blendstate">ID3D10BlendState</a>. <b>ID3D10BlendState1</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ID3D10BlendState1</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/edddc555-47f2-4baa-8312-8ececafca07a">GetDesc1</a>
</td>
<td align="left" width="63%">
Get the blend state.

</td>
</tr>
</table> 


## -remarks



Blending combines two pixel values. You have control over how the pixels are blended by using a predefined set of blending operations, as well as preblending operations. The <a href="https://docs.microsoft.com/windows/desktop/direct3d11/d3d10-graphics-programming-guide-output-merger-stage">Blending Block Diagram</a> shows conceptually how blending works.

To create a blend-state interface, call <a href="https://docs.microsoft.com/windows/desktop/api/d3d10_1/nf-d3d10_1-id3d10device1-createblendstate1">ID3D10Device1::CreateBlendState1</a>. To initialize the blend state, call <a href="https://docs.microsoft.com/windows/desktop/api/d3d10/nf-d3d10-id3d10device-omsetblendstate">ID3D10Device::OMSetBlendState</a>.

This method requires Windows Vista Service Pack 1.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/direct3d10/d3d10-graphics-reference-d3d10-core-interfaces">Core Interfaces</a>



<a href="https://docs.microsoft.com/windows/desktop/api/d3d10/nn-d3d10-id3d10blendstate">ID3D10BlendState</a>
 

 

