---
title: Aspose::Page::XPS::XpsDocument::CreatePolyLineSegment method
linktitle: CreatePolyLineSegment
second_title: Aspose.Page for C++
description: 'Aspose::Page::XPS::XpsDocument::CreatePolyLineSegment method. Creates a new polygonal drawing containing an arbitrary number of individual vertices in C++.'
type: docs
weight: 2500
url: /cpp/aspose.page.xps/xpsdocument/createpolylinesegment/
---
## XpsDocument::CreatePolyLineSegment method


Creates a new polygonal drawing containing an arbitrary number of individual vertices.

```cpp
System::SharedPtr<XpsModel::XpsPolyLineSegment> Aspose::Page::XPS::XpsDocument::CreatePolyLineSegment(System::ArrayPtr<System::Drawing::PointF> points, bool isStroked=true)
```


| Parameter | Type | Description |
| --- | --- | --- |
| points | System::ArrayPtr\<System::Drawing::PointF\> | A set of coordinates for the multiple segments that define the poly line segment. |
| isStroked | bool | Specifies whether the stroke for this segment of the path is drawn. |

### ReturnValue

New polygonal drawing segment.

## See Also

* Typedef [SharedPtr](../../../system/sharedptr/)
* Class [XpsPolyLineSegment](../../../aspose.page.xps.xpsmodel/xpspolylinesegment/)
* Typedef [ArrayPtr](../../../system/arrayptr/)
* Class [PointF](../../../system.drawing/pointf/)
* Class [XpsDocument](../)
* Namespace [Aspose::Page::XPS](../../)
* Library [Aspose.Page for C++](../../../)
