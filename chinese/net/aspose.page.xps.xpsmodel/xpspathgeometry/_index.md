---
title: XpsPathGeometry
second_title: Aspose.Page for .NET API 参考
description: 封装 PathGeometry 属性元素特征的类 此元素包含一组路径图形这些路径图形可以使用Figures 属性或 使用子 PathFigure 元素指定
type: docs
weight: 1170
url: /zh/net/aspose.page.xps.xpsmodel/xpspathgeometry/
---
## XpsPathGeometry class

封装 PathGeometry 属性元素特征的类。 此元素包含一组路径图形，这些路径图形可以使用Figures 属性或 使用子 PathFigure 元素指定。

```csharp
public sealed class XpsPathGeometry : XpsArray<XpsPathFigure>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Count](../../aspose.page.xps.xpsmodel/xpsarray`1/count) { get; } |  |
| [FillRule](../../aspose.page.xps.xpsmodel/xpspathgeometry/fillrule) { get; set; } | 返回/设置指定几何 形状的相交区域如何组合以形成区域的值。 |
| [Item](../../aspose.page.xps.xpsmodel/xpsarray`1/item) { get; } |  |
| [PathFigures](../../aspose.page.xps.xpsmodel/xpspathgeometry/pathfigures) { get; } | 返回子路径图的列表。 |
| [Transform](../../aspose.page.xps.xpsmodel/xpspathgeometry/transform) { get; set; } | 返回/设置建立局部矩阵变换 的仿射变换矩阵，应用于路径几何的所有子元素和后代元素使用 填充、剪裁或描边。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.page.xps.xpsmodel/xpsarray`1/add)(XpsPathFigure) |  |
| [AddSegment](../../aspose.page.xps.xpsmodel/xpspathgeometry/addsegment)(XpsPathSegment) | 将路径段添加到最后一个 pah 图形的子段列表中。 |
| [Clone](../../aspose.page.xps.xpsmodel/xpspathgeometry/clone)() | 克隆此路径几何。 |
| [Insert](../../aspose.page.xps.xpsmodel/xpsarray`1/insert)(int, XpsPathFigure) |  |
| [InsertSegment](../../aspose.page.xps.xpsmodel/xpspathgeometry/insertsegment)(int, XpsPathSegment) | 在*index*位置的最后一个路径图 的子段列表中插入一个路径段。 |
| [Remove](../../aspose.page.xps.xpsmodel/xpsarray`1/remove)(XpsPathFigure) |  |
| [RemoveAt](../../aspose.page.xps.xpsmodel/xpsarray`1/removeat)(int) |  |
| [RemoveSegment](../../aspose.page.xps.xpsmodel/xpspathgeometry/removesegment)(XpsPathSegment) | 从最后一个路径图的子段列表中删除一个路径段。 |
| [RemoveSegmentAt](../../aspose.page.xps.xpsmodel/xpspathgeometry/removesegmentat)(int) | 从 最后一个路径图*index*位置的子段列表中删除一个路径段。 |

### 也可以看看

* class [XpsArray&lt;T&gt;](../xpsarray-1)
* class [XpsPathFigure](../xpspathfigure)
* 命名空间 [Aspose.Page.XPS.XpsModel](../../aspose.page.xps.xpsmodel)
* 部件 [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->