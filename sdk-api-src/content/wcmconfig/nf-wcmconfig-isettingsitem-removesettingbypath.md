---
UID: NF:wcmconfig.ISettingsItem.RemoveSettingByPath
title: ISettingsItem::RemoveSettingByPath (wcmconfig.h)
description: Removes a setting object specified by its path.helpviewer_keywords: ["ISettingsItem interface [SMI]","RemoveSettingByPath method","ISettingsItem.RemoveSettingByPath","ISettingsItem::RemoveSettingByPath","RemoveSettingByPath","RemoveSettingByPath method [SMI]","RemoveSettingByPath method [SMI]","ISettingsItem interface","smi.isettingsitem_removesettingbypath","wcmconfig/ISettingsItem::RemoveSettingByPath"]
old-location: smi\isettingsitem_removesettingbypath.htm
tech.root: SMI
ms.assetid: 5613df85-009f-4aab-91bc-797a6cf73cd0
ms.date: 12/05/2018
ms.keywords: ISettingsItem interface [SMI],RemoveSettingByPath method, ISettingsItem.RemoveSettingByPath, ISettingsItem::RemoveSettingByPath, RemoveSettingByPath, RemoveSettingByPath method [SMI], RemoveSettingByPath method [SMI],ISettingsItem interface, smi.isettingsitem_removesettingbypath, wcmconfig/ISettingsItem::RemoveSettingByPath
f1_keywords:
- wcmconfig/ISettingsItem.RemoveSettingByPath
dev_langs:
- c++
req.header: wcmconfig.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WcmConfig.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: SMIEngine.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- SMIEngine.dll
api_name:
- ISettingsItem.RemoveSettingByPath
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ISettingsItem::RemoveSettingByPath


## -description


Removes a setting object specified by its path. Unlike GetSettingByPath, the use of <b>ISettingsItem::RemoveSettingByPath</b> is not advocated for attributes.


## -parameters




### -param Path [in]

The path of the item to remove. The path is relative to the current item. 


## -returns



This method can return one of these values.

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
Indicates success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WCM_E_STATENODENOTFOUND </b></dt>
</dl>
</td>
<td width="60%">
Indicates an attempt to remove an item that does not exist.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>HRESULT_FROM_WIN32 (ERROR_INVALID_OPERATION)</b></dt>
</dl>
</td>
<td width="60%">
Indicates an attempt to remove an element that is not a list element.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WCM_E_READONLYITEM </b></dt>
</dl>
</td>
<td width="60%">
Indicates that the item cannot be written, either because  it is a read-only item, or because the namespace was opened in ReadOnly mode.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WCM_E_WRONGESCAPESTRING</b></dt>
</dl>
</td>
<td width="60%">
Indicates that the path contains an unrecognized XML escape sequence.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WCM_E_INVALIDPATH</b></dt>
</dl>
</td>
<td width="60%">
Indicates that the path is incorrectly formatted.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WCM_E_INVALIDKEY </b></dt>
</dl>
</td>
<td width="60%">
Indicates that the path is incorrectly specified and references the wrong key for the list item.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/wcmconfig/nn-wcmconfig-isettingsitem">ISettingsItem</a>
 

 

