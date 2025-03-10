---
UID: NN:appxpackaging.IAppxEncryptionFactory4
title: IAppxEncryptionFactory4 (appxpackaging.h)
description: Creates objects for encrypting Windows app packages and bundles.helpviewer_keywords: ["IAppxEncryptionFactory4","IAppxEncryptionFactory4 interface [App packaging and management]","IAppxEncryptionFactory4 interface [App packaging and management]","described","appxpackaging/IAppxEncryptionFactory4","appxpkg.iappxencryptionfactory4"]
old-location: appxpkg\iappxencryptionfactory4.htm
tech.root: appxpkg
ms.assetid: BEB6BD9B-C265-4C92-98AD-59344B5274D4
ms.date: 12/05/2018
ms.keywords: IAppxEncryptionFactory4, IAppxEncryptionFactory4 interface [App packaging and management], IAppxEncryptionFactory4 interface [App packaging and management],described, appxpackaging/IAppxEncryptionFactory4, appxpkg.iappxencryptionfactory4
f1_keywords:
- appxpackaging/IAppxEncryptionFactory4
dev_langs:
- c++
req.header: appxpackaging.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: AppxPackaging.idl
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
- AppxPackaging.h
api_name:
- IAppxEncryptionFactory4
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAppxEncryptionFactory4 interface


## -description


Creates objects for encrypting Windows app packages and bundles.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAppxEncryptionFactory4</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IAppxEncryptionFactory4</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IAppxEncryptionFactory4</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/appxpackaging/nf-appxpackaging-iappxencryptionfactory4-encryptpackage">EncryptPackage</a>
</td>
<td align="left" width="63%">
Creates an encrypted Windows app package from an unencrypted one.

</td>
</tr>
</table> 

