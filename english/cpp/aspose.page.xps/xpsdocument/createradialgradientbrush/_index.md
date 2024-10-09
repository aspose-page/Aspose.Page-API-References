---
title: Aspose::Page::XPS::XpsDocument::CreateRadialGradientBrush method
linktitle: CreateRadialGradientBrush
second_title: Aspose.Page for C++
description: 'Aspose::Page::XPS::XpsDocument::CreateRadialGradientBrush method. Creates a new radial gradient brush in C++.'
type: docs
weight: 2700
url: /cpp/aspose.page.xps/xpsdocument/createradialgradientbrush/
---
## XpsDocument::CreateRadialGradientBrush(System::Drawing::PointF, System::Drawing::PointF, float, float) method


Creates a new radial gradient brush.

```cpp
System::SharedPtr<XpsModel::XpsRadialGradientBrush> Aspose::Page::XPS::XpsDocument::CreateRadialGradientBrush(System::Drawing::PointF center, System::Drawing::PointF gradientOrigin, float radiusX, float radiusY)
```


| Parameter | Type | Description |
| --- | --- | --- |
| center | System::Drawing::PointF | The center point of the radial gradient (that is, the center of the ellipse). |
| gradientOrigin | System::Drawing::PointF | The origin point of the radial gradient. |
| radiusX | float | The radius in the x dimension of the ellipse which defines the radial gradient. |
| radiusY | float | The radius in the y dimension of the ellipse which defines the radial gradient. |

### ReturnValue

New radial gradient brush.

## See Also

* Typedef [SharedPtr](../../../system/sharedptr/)
* Class [XpsRadialGradientBrush](../../../aspose.page.xps.xpsmodel/xpsradialgradientbrush/)
* Class [PointF](../../../system.drawing/pointf/)
* Class [XpsDocument](../)
* Namespace [Aspose::Page::XPS](../../)
* Library [Aspose.Page for C++](../../../)
## XpsDocument::CreateRadialGradientBrush(System::SharedPtr\<System::Collections::Generic::List\<System::SharedPtr\<XpsModel::XpsGradientStop\>\>\>, System::Drawing::PointF, System::Drawing::PointF, float, float) method


Creates a new radial gradient brush.

```cpp
System::SharedPtr<XpsModel::XpsRadialGradientBrush> Aspose::Page::XPS::XpsDocument::CreateRadialGradientBrush(System::SharedPtr<System::Collections::Generic::List<System::SharedPtr<XpsModel::XpsGradientStop>>> gradientStops, System::Drawing::PointF center, System::Drawing::PointF gradientOrigin, float radiusX, float radiusY)
```


| Parameter | Type | Description |
| --- | --- | --- |
| gradientStops | System::SharedPtr\<System::Collections::Generic::List\<System::SharedPtr\<XpsModel::XpsGradientStop\>\>\> | The list of gradient stops. |
| center | System::Drawing::PointF | The center point of the radial gradient (that is, the center of the ellipse). |
| gradientOrigin | System::Drawing::PointF | The origin point of the radial gradient. |
| radiusX | float | The radius in the x dimension of the ellipse which defines the radial gradient. |
| radiusY | float | The radius in the y dimension of the ellipse which defines the radial gradient. |

### ReturnValue

New radial gradient brush.

## See Also

* Typedef [SharedPtr](../../../system/sharedptr/)
* Class [XpsRadialGradientBrush](../../../aspose.page.xps.xpsmodel/xpsradialgradientbrush/)
* Class [List](../../../system.collections.generic/list/)
* Class [XpsGradientStop](../../../aspose.page.xps.xpsmodel/xpsgradientstop/)
* Class [PointF](../../../system.drawing/pointf/)
* Class [XpsDocument](../)
* Namespace [Aspose::Page::XPS](../../)
* Library [Aspose.Page for C++](../../../)
