---
UID: NF:uiautomationclient.IUIAutomationTableItemPattern.GetCurrentRowHeaderItems
title: IUIAutomationTableItemPattern::GetCurrentRowHeaderItems (uiautomationclient.h)
description: Retrieves the row headers associated with a table item or cell.helpviewer_keywords: ["GetCurrentRowHeaderItems","GetCurrentRowHeaderItems method [Windows Accessibility]","GetCurrentRowHeaderItems method [Windows Accessibility]","IUIAutomationTableItemPattern interface","IUIAutomationTableItemPattern interface [Windows Accessibility]","GetCurrentRowHeaderItems method","IUIAutomationTableItemPattern.GetCurrentRowHeaderItems","IUIAutomationTableItemPattern::GetCurrentRowHeaderItems","uiauto.uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems","uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems","uiautomationclient/IUIAutomationTableItemPattern::GetCurrentRowHeaderItems","winauto.uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems"]
old-location: winauto\uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems.htm
tech.root: WinAuto
ms.assetid: 6ae074c6-1855-4aea-845c-284a7bbc3f3f
ms.date: 12/05/2018
ms.keywords: GetCurrentRowHeaderItems, GetCurrentRowHeaderItems method [Windows Accessibility], GetCurrentRowHeaderItems method [Windows Accessibility],IUIAutomationTableItemPattern interface, IUIAutomationTableItemPattern interface [Windows Accessibility],GetCurrentRowHeaderItems method, IUIAutomationTableItemPattern.GetCurrentRowHeaderItems, IUIAutomationTableItemPattern::GetCurrentRowHeaderItems, uiauto.uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems, uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems, uiautomationclient/IUIAutomationTableItemPattern::GetCurrentRowHeaderItems, winauto.uiauto_IUIAutomationTableItemPattern_GetCurrentRowHeaderItems
f1_keywords:
- uiautomationclient/IUIAutomationTableItemPattern.GetCurrentRowHeaderItems
dev_langs:
- c++
req.header: uiautomationclient.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista, Windows XP with SP3 and Platform Update for Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008, Windows Server 2003 with SP2 and Platform Update for Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationClient.idl
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
- UIAutomationClient.h
api_name:
- IUIAutomationTableItemPattern.GetCurrentRowHeaderItems
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IUIAutomationTableItemPattern::GetCurrentRowHeaderItems


## -description


Retrieves the row headers associated with a table item or cell.


## -parameters




### -param retVal [out, retval]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/uiautomationclient/nn-uiautomationclient-iuiautomationelementarray">IUIAutomationElementArray</a>**</b>

Receives a pointer to the collection of row headers.


## -returns



Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



