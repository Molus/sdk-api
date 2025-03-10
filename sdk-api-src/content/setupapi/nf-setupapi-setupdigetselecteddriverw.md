---
UID: NF:setupapi.SetupDiGetSelectedDriverW
title: SetupDiGetSelectedDriverW function (setupapi.h)
description: The SetupDiGetSelectedDriver function retrieves the selected driver for a device information set or a particular device information element.helpviewer_keywords: ["SetupDiGetSelectedDriver","SetupDiGetSelectedDriver function [Device and Driver Installation]","SetupDiGetSelectedDriverA","SetupDiGetSelectedDriverW","devinst.setupdigetselecteddriver","di-rtns_6ea54b58-1b3f-4437-afa0-501a23af3529.xml","setupapi/SetupDiGetSelectedDriver"]
old-location: devinst\setupdigetselecteddriver.htm
tech.root: devinst
ms.assetid: dd3d9736-755c-497c-a523-18ca66557ae7
ms.date: 12/05/2018
ms.keywords: SetupDiGetSelectedDriver, SetupDiGetSelectedDriver function [Device and Driver Installation], SetupDiGetSelectedDriverA, SetupDiGetSelectedDriverW, devinst.setupdigetselecteddriver, di-rtns_6ea54b58-1b3f-4437-afa0-501a23af3529.xml, setupapi/SetupDiGetSelectedDriver
f1_keywords:
- setupapi/SetupDiGetSelectedDriver
dev_langs:
- c++
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
req.lib: Setupapi.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- LibDef
api_location:
- Setupapi.lib
- Setupapi.dll
api_name:
- SetupDiGetSelectedDriver - SetupDiGetSelectedDriverW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SetupDiGetSelectedDriverW function


## -description


The <b>SetupDiGetSelectedDriver</b> function retrieves the selected driver for a device information set or a particular device information element.


## -parameters




### -param DeviceInfoSet [in]

A handle to the <a href="https://docs.microsoft.com/windows-hardware/drivers/install/device-information-sets">device information set</a> for which to retrieve a selected driver.


### -param DeviceInfoData [in, optional]

A pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/setupapi/ns-setupapi-sp_devinfo_data">SP_DEVINFO_DATA</a> structure that specifies a device information element that represents the device in <i>DeviceInfoSet</i> for which to retrieve the selected driver. This parameter is optional and can be <b>NULL</b>. If this parameter is specified, <b>SetupDiGetSelectedDriver</b> retrieves the selected driver for the specified device. If this parameter is <b>NULL</b>, <b>SetupDiGetSelectedDriver</b> retrieves the selected class driver in the global class driver list that is associated with <i>DeviceInfoSet</i>. 


### -param DriverInfoData [out]

A pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/setupapi/ns-setupapi-sp_drvinfo_data_v1_a">SP_DRVINFO_DATA</a> structure that receives information about the selected driver.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved with a call to <a href="https://msdn.microsoft.com/library/ms679360(VS.85).aspx">GetLastError</a>. If a driver has not been selected for the specified device instance, the logged error is ERROR_NO_DRIVER_SELECTED.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdisetselecteddrivera">SetupDiSetSelectedDriver</a>
 

 

