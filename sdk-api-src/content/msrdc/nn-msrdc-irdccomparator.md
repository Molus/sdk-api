---
UID: NN:msrdc.IRdcComparator
title: IRdcComparator (msrdc.h)
description: Used to compare two signature streams (seed and source) and produce the list of source and seed file data chunks needed to create the target file.helpviewer_keywords: ["IRdcComparator","IRdcComparator interface [Remote Differential Compression]","IRdcComparator interface [Remote Differential Compression]","described","fs.irdccomparator","msrdc/IRdcComparator","rdc.irdccomparator"]
old-location: rdc\irdccomparator.htm
tech.root: rdc
ms.assetid: ad39b922-3271-491e-b74b-80a1f647e663
ms.date: 12/05/2018
ms.keywords: IRdcComparator, IRdcComparator interface [Remote Differential Compression], IRdcComparator interface [Remote Differential Compression],described, fs.irdccomparator, msrdc/IRdcComparator, rdc.irdccomparator
f1_keywords:
- msrdc/IRdcComparator
dev_langs:
- c++
req.header: msrdc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: MsRdc.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: MsRdc.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- MsRdc.dll
api_name:
- IRdcComparator
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IRdcComparator interface


## -description


The <b>IRdcComparator</b> interface is used to compare 
    two signature streams (seed and source) and produce the list of source and seed file data chunks needed to create the target 
    file.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IRdcComparator</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IRdcComparator</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IRdcComparator</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="inherited;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/msrdc/nf-msrdc-irdccomparator-process">Process</a>
</td>
<td align="left" width="63%">
Compares two signature streams (seed and source) and produces a needs list, which describes the data chunks needed to create 
    the target file.</p> (Inherited from <b>IRdcComparator</b>)</td>
</tr>
</table> 


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/rdc/remote-differential-compression-interfaces">Remote Differential Compression Interfaces</a>
 

 

