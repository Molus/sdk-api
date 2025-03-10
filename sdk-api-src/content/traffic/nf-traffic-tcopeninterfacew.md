---
UID: NF:traffic.TcOpenInterfaceW
title: TcOpenInterfaceW function (traffic.h)
description: The TcOpenInterface function opens an interface.helpviewer_keywords: ["TcOpenInterface","TcOpenInterface function [QOS]","TcOpenInterfaceA","TcOpenInterfaceW","_gqos_tcopeninterface","qos.tcopeninterface","traffic/TcOpenInterface","traffic/TcOpenInterfaceA","traffic/TcOpenInterfaceW"]
old-location: qos\tcopeninterface.htm
tech.root: QOS
ms.assetid: 8c7e658c-862f-4715-9ba5-ac079db924a1
ms.date: 12/05/2018
ms.keywords: TcOpenInterface, TcOpenInterface function [QOS], TcOpenInterfaceA, TcOpenInterfaceW, _gqos_tcopeninterface, qos.tcopeninterface, traffic/TcOpenInterface, traffic/TcOpenInterfaceA, traffic/TcOpenInterfaceW
f1_keywords:
- traffic/TcOpenInterface
dev_langs:
- c++
req.header: traffic.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: TcOpenInterfaceW (Unicode) and TcOpenInterfaceA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Traffic.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Traffic.dll
api_name:
- TcOpenInterface
- TcOpenInterfaceA
- TcOpenInterfaceW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# TcOpenInterfaceW function


## -description


The 
<b>TcOpenInterface</b> function opens an interface. The 
<b>TcOpenInterface</b> function identifies and opens an interface based on its text string, which is available from a call to 
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/traffic/nf-traffic-tcenumerateinterfaces">TcEnumerateInterfaces</a>. Once an interface is opened, the client must be prepared to receive notification regarding the open interface, through traffic control's use of the interface context.


## -parameters




### -param pInterfaceName [in]

Pointer to the text string identifying the interface to be opened. This text string is part of the information returned in a previous call to 
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/traffic/nf-traffic-tcenumerateinterfaces">TcEnumerateInterfaces</a>.


### -param ClientHandle [in]

Handle used by traffic control to identify the client, obtained through the <i>pClientHandle</i> parameter of the client's call to 
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/traffic/nf-traffic-tcregisterclient">TcRegisterClient</a>.


### -param ClIfcCtx [in]

Client's interface–context handle for the opened interface. Used as a callback parameter by traffic control when communicating with the client about the opened interface. This can be a container to hold an arbitrary client-defined context for this instance of the interface.


### -param pIfcHandle [out]

Pointer to the buffer where traffic control can return an interface handle. The interface handle returned to <i>pIfcHandle</i> must be used by the client to identify the interface in subsequent calls to traffic control.


## -returns



<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>NO_ERROR</b></dt>
</dl>
</td>
<td width="60%">
The function executed without errors.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One of the parameters is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
The system is out of memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
Traffic control failed to find an interface with the name provided in <i>pInterfaceName</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
The client handle is invalid.

</td>
</tr>
</table>
 




## -remarks



Use of the 
<b>TcOpenInterface</b> function requires administrative privilege.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/traffic/nc-traffic-tci_notify_handler">ClNotifyHandler</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/traffic/nf-traffic-tcenumerateinterfaces">TcEnumerateInterfaces</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/traffic/nf-traffic-tcregisterclient">TcRegisterClient</a>
 

 

