---
UID: NF:d2d1.ID2D1RenderTarget.DrawEllipse(const D2D1_ELLIPSE &,ID2D1Brush,FLOAT,ID2D1StrokeStyle)
title: ID2D1RenderTarget::DrawEllipse(const D2D1_ELLIPSE &,ID2D1Brush,FLOAT,ID2D1StrokeStyle) (d2d1.h)
description: Draws the outline of the specified ellipse using the specified stroke style.
helpviewer_keywords: ["DrawEllipse","DrawEllipse method [Direct2D]","DrawEllipse method [Direct2D]","ID2D1RenderTarget interface","ID2D1RenderTarget interface [Direct2D]","DrawEllipse method","ID2D1RenderTarget.DrawEllipse","ID2D1RenderTarget.DrawEllipse(const D2D1_ELLIPSE &","ID2D1Brush","FLOAT","ID2D1StrokeStyle)","ID2D1RenderTarget::DrawEllipse","ID2D1RenderTarget::DrawEllipse(const D2D1_ELLIPSE &","ID2D1Brush","FLOAT","ID2D1StrokeStyle)","d2d1/ID2D1RenderTarget::DrawEllipse","direct2d.ID2D1RenderTarget_DrawEllipse_ref_D2D1_ELLIPSE_ptr_ID2D1Brush_FLOAT_ptr_ID2D1StrokeStyle"]
old-location: direct2d\ID2D1RenderTarget_DrawEllipse_ref_D2D1_ELLIPSE_ptr_ID2D1Brush_FLOAT_ptr_ID2D1StrokeStyle.htm
tech.root: Direct2D
ms.assetid: 3cd3aad6-72fc-41a3-a792-6ecac838c080
ms.date: 12/05/2018
ms.keywords: DrawEllipse, DrawEllipse method [Direct2D], DrawEllipse method [Direct2D],ID2D1RenderTarget interface, ID2D1RenderTarget interface [Direct2D],DrawEllipse method, ID2D1RenderTarget.DrawEllipse, ID2D1RenderTarget.DrawEllipse(const D2D1_ELLIPSE &,ID2D1Brush,FLOAT,ID2D1StrokeStyle), ID2D1RenderTarget::DrawEllipse, ID2D1RenderTarget::DrawEllipse(const D2D1_ELLIPSE &,ID2D1Brush,FLOAT,ID2D1StrokeStyle), d2d1/ID2D1RenderTarget::DrawEllipse, direct2d.ID2D1RenderTarget_DrawEllipse_ref_D2D1_ELLIPSE_ptr_ID2D1Brush_FLOAT_ptr_ID2D1StrokeStyle
f1_keywords:
- d2d1/ID2D1RenderTarget.DrawEllipse
dev_langs:
- c++
req.header: d2d1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D2d1.lib
req.dll: D2d1.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D2d1.dll
api_name:
- ID2D1RenderTarget.DrawEllipse
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

## -description

Draws the outline of the specified ellipse using the specified stroke style.

## -parameters

### -param ellipse

Type: [in] <b>const <a href="/windows/win32/api/d2d1/ns-d2d1-d2d1_ellipse">D2D1_ELLIPSE</a> &</b>

The position and radius of the ellipse to draw, in device-independent pixels.

### -param brush

Type: [in] <b><a href="/windows/win32/api/d2d1/nn-d2d1-id2d1brush">ID2D1Brush</a>*</b>

The brush used to paint the ellipse's outline.

### -param strokeWidth

Type: [in] <b>FLOAT</b>

The width of the stroke, in device-independent pixels. The value must be greater than or equal to 0.0f. If this parameter isn't specified, it defaults to 1.0f. The stroke is centered on the line.

### -param strokeStyle

Type: [in, optional] <b><a href="/windows/win32/api/d2d1/nn-d2d1-id2d1strokestyle">ID2D1StrokeStyle</a>*</b>

The style of stroke to apply to the ellipse's outline, or <b>NULL</b> to paint a solid stroke.

## -remarks

The <a href="/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-drawellipse(constd2d1_ellipse_id2d1brush_float_id2d1strokestyle)">DrawEllipse</a> method doesn't return an error code if it fails. To determine whether a drawing operation (such as <b>DrawEllipse</b>) failed, check the result returned by the <a href="/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-enddraw">ID2D1RenderTarget::EndDraw</a> or <a href="/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-flush">ID2D1RenderTarget::Flush</a> methods. 

## Examples

For an example, see <a href="/windows/win32/Direct2D/how-to-draw-an-ellipse">How to Draw and Fill a Basic Shape</a>.

## -see-also

<a href="/windows/win32/api/d2d1/nn-d2d1-id2d1rendertarget">ID2D1RenderTarget</a>