---
UID: NN:portabledeviceapi.IPortableDevice
title: IPortableDevice (portabledeviceapi.h)
description: The IPortableDevice interface provides access to a portable device.
old-location: wpdsdk\iportabledevice.htm
tech.root: wpd_sdk
ms.assetid: 98c48e56-56b8-4800-b52b-ac08f2abf27e
ms.date: 12/05/2018
ms.keywords: IPortableDevice, IPortableDevice interface [Windows Portable Devices SDK], IPortableDevice interface [Windows Portable Devices SDK],described, IPortableDeviceInterface, portabledeviceapi/IPortableDevice, wpdsdk.iportabledevice
ms.topic: interface
f1_keywords:
- portabledeviceapi/IPortableDevice
dev_langs:
- c++
req.header: portabledeviceapi.h
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
req.lib: PortableDeviceGUIDs.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
api_name:
- IPortableDevice
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPortableDevice interface


## -description


The <b>IPortableDevice</b> interface provides access to a portable device.

To create and open this interface, first call <a href="https://docs.microsoft.com/windows/desktop/api/combaseapi/nf-combaseapi-cocreateinstance">CoCreateInstance</a> with <b>CLSID_PortableDeviceFTM</b>  or <b>CLSID_PortableDevice</b>to retrieve an <b>IPortableDevice</b> interface, and then call <a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-open">Open</a> to open a connection to the device.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IPortableDevice</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IPortableDevice</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IPortableDevice</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-advise">Advise</a>
</td>
<td align="left" width="63%">
Registers an application-defined callback that receives device events.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-cancel">Cancel</a>
</td>
<td align="left" width="63%">
Cancels a pending operation on this interface.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-capabilities">Capabilities</a>
</td>
<td align="left" width="63%">
Retrieves an interface used to query the capabilities of a portable device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-close">Close</a>
</td>
<td align="left" width="63%">
Closes the connection with the device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-content">Content</a>
</td>
<td align="left" width="63%">
Retrieves an interface used to access objects on a device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-getpnpdeviceid">GetPnPDeviceID</a>
</td>
<td align="left" width="63%">
Retrieves a Plug-and-Play (PnP) identifier used to open a device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-open">Open</a>
</td>
<td align="left" width="63%">
Opens a connection between the application and the device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-sendcommand">SendCommand</a>
</td>
<td align="left" width="63%">
Sends a command to the device and retrieves the results synchronously.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nf-portabledeviceapi-iportabledevice-unadvise">Unadvise</a>
</td>
<td align="left" width="63%">
Unregisters a client from receiving callback notifications.

</td>
</tr>
</table> 


## -remarks



The client interfaces are designed to be used for any WPD object; it is not necessary to create a new instance for each object referenced by the application. After an application opens an instance of the <b>IPortableDevice</b> interface, it should open and cache any other WPD client interfaces that it will require.
      

For Windows 7, <a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nn-portabledeviceapi-iportabledeviceservice">IPortableDevice</a> supports two CLSIDs for <b>CoCreateInstance</b>. <b>CLSID_PortableDevice</b> returns an <b>IPortableDevice</b> pointer that does not aggregate the free-threaded marshaler; <b>CLSID_PortableDeviceFTM</b> is a new CLSID that returns an <b>IPortableDevice</b> pointer that aggregates the free-threaded marshaler.  Both pointers support the same functionality otherwise.

Applications that live in Single Threaded Apartments should use <b>CLSID_PortableDeviceFTM</b> as this eliminates the overhead of interface pointer marshaling.  <b>CLSID_PortableDevice</b> is still supported for legacy applications.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/wpd_sdk/client-interfaces">Client Interfaces</a>
 

 

