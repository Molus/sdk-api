---
UID: NF:fdi.FNWRITE
title: FNWRITE macro (fdi.h)
description: The FNWRITE macro provides the declaration for the application-defined callback function to write data to a file in an FDI context.helpviewer_keywords: ["FNWRITE","FNWRITE macro [Windows API]","fdi/FNWRITE","winprog.fnwrite"]
old-location: winprog\fnwrite.htm
tech.root: DevNotes
ms.assetid: e15d4293-2955-48cd-b8c9-77669a1e6436
ms.date: 12/05/2018
ms.keywords: FNWRITE, FNWRITE macro [Windows API], fdi/FNWRITE, winprog.fnwrite
f1_keywords:
- fdi/FNWRITE
dev_langs:
- c++
req.header: fdi.h
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
- HeaderDef
api_location:
- fdi.h
api_name:
- FNWRITE
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# FNWRITE macro


## -description


The <b>FNWRITE</b> macro provides the declaration for the application-defined callback function to write data to a file in an FDI context.


## -parameters




### -param fn [in]

An application-defined value used to identify the open file.


#### - cb

The maximum number of bytes to be written.


#### - pv [in]

Pointer to the buffer containing the data to be written.


## -remarks



The function accepts parameters similar to <a href="https://msdn.microsoft.com/library/1570wh78(VS.80).aspx">_write</a>.


#### Examples


```cpp
FNWRITE(fnFileWrite)
{
    DWORD dwBytesWritten = 0;

    if ( WriteFile((HANDLE)hf, pv, cb, &dwBytesWritten, NULL) == FALSE )
    {
        dwBytesWritten = (DWORD)-1;
    }

    return dwBytesWritten;
}

```





## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/fdi/nf-fdi-fdicreate">FDICreate</a>
 

 

