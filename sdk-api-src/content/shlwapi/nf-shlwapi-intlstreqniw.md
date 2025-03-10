---
UID: NF:shlwapi.IntlStrEqNIW
title: IntlStrEqNIW macro (shlwapi.h)
description: Performs a case-insensitive comparison of a specified number of characters from the beginning of two localized strings.helpviewer_keywords: ["IntlStrEqNI","IntlStrEqNI function [Windows Shell]","IntlStrEqNIA","IntlStrEqNIW","_win32_IntlStrEqNI","shell.IntlStrEqNI","shlwapi/IntlStrEqNI","shlwapi/IntlStrEqNIA","shlwapi/IntlStrEqNIW"]
old-location: shell\IntlStrEqNI.htm
tech.root: shell
ms.assetid: 3d201726-b24a-4739-84fb-49b54d3f0f07
ms.date: 12/05/2018
ms.keywords: IntlStrEqNI, IntlStrEqNI function [Windows Shell], IntlStrEqNIA, IntlStrEqNIW, _win32_IntlStrEqNI, shell.IntlStrEqNI, shlwapi/IntlStrEqNI, shlwapi/IntlStrEqNIA, shlwapi/IntlStrEqNIW
f1_keywords:
- shlwapi/IntlStrEqNI
dev_langs:
- c++
req.header: shlwapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: IntlStrEqNIW (Unicode) and IntlStrEqNIA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Shlwapi.lib
req.dll: Shlwapi.dll (version 5.0 or later)
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Shlwapi.dll
api_name:
- IntlStrEqNI
- IntlStrEqNIA
- IntlStrEqNIW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IntlStrEqNIW macro


## -description


Performs a case-insensitive comparison of a specified number of characters from the beginning of two localized strings.


## -parameters




### -param s1 [in]

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string.


### -param s2 [in]

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string.


### -param nChar [in]

Type: <b>int</b>

The number of characters to be compared, starting from the beginning of the strings.


## -remarks



This function retrieves the thread locale and uses <a href="https://docs.microsoft.com/windows/desktop/api/stringapiset/nf-stringapiset-comparestringw">CompareString</a> to do a case-insensitive comparison of the first <i>nChar</i> characters. It is equivalent to:

<pre class="syntax" xml:space="preserve"><code>IntlStrEqWorker(FALSE, pszStr1, pszStr2, nChar)</code></pre>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/shlwapi/nf-shlwapi-intlstreqworkera">IntlStrEqWorker</a>
 

 

