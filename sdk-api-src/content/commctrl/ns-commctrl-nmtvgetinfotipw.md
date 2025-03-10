---
UID: NS:commctrl.tagNMTVGETINFOTIPW
title: NMTVGETINFOTIPW (commctrl.h)
description: Contains and receives tree-view item information needed to display a tooltip for an item. This structure is used with the TVN_GETINFOTIP notification code.helpviewer_keywords: ["*LPNMTVGETINFOTIPW","LPNMTVGETINFOTIP","LPNMTVGETINFOTIP structure pointer [Windows Controls]","NMTVGETINFOTIP","NMTVGETINFOTIP structure [Windows Controls]","NMTVGETINFOTIPA","NMTVGETINFOTIPW","_win32_NMTVGETINFOTIP","_win32_NMTVGETINFOTIP_cpp","commctrl/LPNMTVGETINFOTIP","commctrl/NMTVGETINFOTIP","commctrl/NMTVGETINFOTIPA","commctrl/NMTVGETINFOTIPW","controls.NMTVGETINFOTIP","controls._win32_NMTVGETINFOTIP"]
old-location: controls\NMTVGETINFOTIP.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\structures\nmtvgetinfotip.htm
ms.date: 12/05/2018
ms.keywords: '*LPNMTVGETINFOTIPW, LPNMTVGETINFOTIP, LPNMTVGETINFOTIP structure pointer [Windows Controls], NMTVGETINFOTIP, NMTVGETINFOTIP structure [Windows Controls], NMTVGETINFOTIPA, NMTVGETINFOTIPW, _win32_NMTVGETINFOTIP, _win32_NMTVGETINFOTIP_cpp, commctrl/LPNMTVGETINFOTIP, commctrl/NMTVGETINFOTIP, commctrl/NMTVGETINFOTIPA, commctrl/NMTVGETINFOTIPW, controls.NMTVGETINFOTIP, controls._win32_NMTVGETINFOTIP'
f1_keywords:
- commctrl/NMTVGETINFOTIP
dev_langs:
- c++
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: NMTVGETINFOTIPW (Unicode) and NMTVGETINFOTIPA (ANSI)
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
- HeaderDef
api_location:
- Commctrl.h
api_name:
- NMTVGETINFOTIP
- NMTVGETINFOTIPA
- NMTVGETINFOTIPW
targetos: Windows
req.typenames: NMTVGETINFOTIPW, *LPNMTVGETINFOTIPW
req.redist: 
ms.custom: 19H1
---

# NMTVGETINFOTIPW structure


## -description


Contains and receives tree-view item information needed to display a tooltip for an item. This structure is used with the <a href="https://docs.microsoft.com/windows/desktop/Controls/tvn-getinfotip">TVN_GETINFOTIP</a> notification code. 


## -struct-fields




### -field hdr

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/richedit/ns-richedit-nmhdr">NMHDR</a></b>


<a href="https://docs.microsoft.com/windows/desktop/api/richedit/ns-richedit-nmhdr">NMHDR</a> structure that contains information about this notification. 


### -field pszText

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">LPTSTR</a></b>

Address of a character buffer that contains the text to be displayed. If you want to change the text displayed in the tooltip, you will need to modify the contents of this buffer. The size of this buffer is specified by the 
					<b>cchTextMax</b> structure. 


### -field cchTextMax

Type: <b>int</b>

Size of the buffer at 
					<b>pszText</b>, in characters. Although you should never assume that this buffer will be of any particular size, the INFOTIPSIZE value can be used for design purposes. 


### -field hItem

Type: <b>HTREEITEM</b>

Tree handle to the item for which the tooltip is being displayed. 


### -field lParam

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">LPARAM</a></b>

Application-defined data associated with the item for which the tooltip is being displayed. 

