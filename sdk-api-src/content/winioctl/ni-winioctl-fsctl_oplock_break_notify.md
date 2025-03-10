---
UID: NI:winioctl.FSCTL_OPLOCK_BREAK_NOTIFY
title: FSCTL_OPLOCK_BREAK_NOTIFY
description: Enables the calling application to wait for completion of an opportunistic lock break.
helpviewer_keywords: ["FSCTL_OPLOCK_BREAK_NOTIFY","FSCTL_OPLOCK_BREAK_NOTIFY control","FSCTL_OPLOCK_BREAK_NOTIFY control code [Files]","_win32_fsctl_oplock_break_notify","base.fsctl_oplock_break_notify","fs.fsctl_oplock_break_notify","winioctl/FSCTL_OPLOCK_BREAK_NOTIFY"]
old-location: fs\fsctl_oplock_break_notify.htm
tech.root: FileIO
ms.assetid: 5d064b92-4d30-4213-a9f0-713fd0e7c321
ms.date: 12/05/2018
ms.keywords: FSCTL_OPLOCK_BREAK_NOTIFY, FSCTL_OPLOCK_BREAK_NOTIFY control, FSCTL_OPLOCK_BREAK_NOTIFY control code [Files], _win32_fsctl_oplock_break_notify, base.fsctl_oplock_break_notify, fs.fsctl_oplock_break_notify, winioctl/FSCTL_OPLOCK_BREAK_NOTIFY
f1_keywords:
- winioctl/FSCTL_OPLOCK_BREAK_NOTIFY
dev_langs:
- c++
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
- WinIoCtl.h
api_name:
- FSCTL_OPLOCK_BREAK_NOTIFY
targetos: Windows
req.typenames: 
req.redist: 
---

# FSCTL_OPLOCK_BREAK_NOTIFY IOCTL

## -description

Enables the calling application to wait for completion of an opportunistic lock break.

This operation is not useful to application developers and is documented here only for completeness. [CreateFile](../fileapi/nf-fileapi-createfilea.md) handles the problem that this operation was designed to handle.

To perform this operation, call the [**DeviceIoControl**](../ioapiset/nf-ioapiset-deviceiocontrol.md) function using the following parameters.

```cpp
BOOL DeviceIoControl(
  (HANDLE) hDevice,             // handle to file
  FSCTL_OPLOCK_BREAK_NOTIFY,    // dwIoControlCode
  NULL,                         // lpInBuffer
  0,                            // nInBufferSize
  NULL,                         // lpOutBuffer
  0,                            // nOutBufferSize
  (LPDWORD) lpBytesReturned,    // number of bytes returned
  (LPOVERLAPPED) lpOverlapped   // OVERLAPPED structure
);
```

## -ioctlparameters

### -input-buffer


### -input-buffer-length


### -output-buffer


### -output-buffer-length


### -in-out-buffer


### -inout-buffer-length


### -status-block

Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [NTSTATUS Values](https://docs.microsoft.com/windows-hardware/drivers/kernel/ntstatus-values).


## -remarks

This operation is used only by client applications that have requested an opportunistic lock from a local server. Client applications requesting opportunistic locks from remote servers must not request them directly—the network redirector transparently requests opportunistic locks for the application.

For the implications of overlapped I/O on this operation, see the Remarks section of the [DeviceIoControl](../ioapiset/nf-ioapiset-deviceiocontrol.md) topic.

In Windows 8 and Windows Server 2012, this code is supported by the following technologies.

Technology | Supported
-----------|----------
Server Message Block (SMB) 3.0 protocol | No
SMB 3.0 Transparent Failover (TFO) | No
SMB 3.0 with Scale-out File Shares (SO) | No
Cluster Shared Volume File System (CsvFS) | Yes
Resilient File System (ReFS) | Yes


## -see-also

* [CreateFile](../fileapi/nf-fileapi-createfilea.md)
* [DeviceIoControl](../ioapiset/nf-ioapiset-deviceiocontrol.md)
* [OVERLAPPED](../minwinbase/ns-minwinbase-overlapped.md)
* [Oplock Semantics](https://docs.microsoft.com/windows-hardware/drivers/ifs/oplock-semantics)
* [Opportunistic Locks](https://docs.microsoft.com/windows/desktop/FileIO/opportunistic-locks)
