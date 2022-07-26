---
title: XpsMatrix
second_title: Aspose.Page for .NET API 参考
description: 封装 MatrixTransform 属性元素特征的类 该元素定义了一个任意仿射矩阵变换用于操作坐标 元素系统
type: docs
weight: 1110
url: /zh/net/aspose.page.xps.xpsmodel/xpsmatrix/
---
## XpsMatrix class

封装 MatrixTransform 属性元素特征的类。 该元素定义了一个任意仿射矩阵变换，用于操作坐标 元素系统。

```csharp
public sealed class XpsMatrix : XpsObject
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [IsIdentity](../../aspose.page.xps.xpsmodel/xpsmatrix/isidentity) { get; } | 获取一个值，该值指示此实例是否为单位矩阵。 |
| [M11](../../aspose.page.xps.xpsmodel/xpsmatrix/m11) { get; } | 获取 M11 元素。 |
| [M12](../../aspose.page.xps.xpsmodel/xpsmatrix/m12) { get; } | 获取 M12 元素。 |
| [M21](../../aspose.page.xps.xpsmodel/xpsmatrix/m21) { get; } | 获取 M21 元素。 |
| [M22](../../aspose.page.xps.xpsmodel/xpsmatrix/m22) { get; } | 获取 M22 元素。 |
| [M31](../../aspose.page.xps.xpsmodel/xpsmatrix/m31) { get; } | 获取 M31 元素。 |
| [M32](../../aspose.page.xps.xpsmodel/xpsmatrix/m32) { get; } | 获取 M32 元素。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Clone](../../aspose.page.xps.xpsmodel/xpsmatrix/clone)() | 克隆这个变换矩阵。 |
| override [Equals](../../aspose.page.xps.xpsmodel/xpsmatrix/equals)(object) | 确定指定的Object是否等于此实例。 |
| override [GetHashCode](../../aspose.page.xps.xpsmodel/xpsmatrix/gethashcode)() | 返回此实例的哈希码。 |
| [Multiply](../../aspose.page.xps.xpsmodel/xpsmatrix/multiply#multiply_2)(Matrix) | 将此矩阵乘以*matrix* 指定的矩阵，默认（前置）顺序。 |
| [Multiply](../../aspose.page.xps.xpsmodel/xpsmatrix/multiply#multiply)(XpsMatrix) | 将此矩阵乘以*matrix* 指定的矩阵，默认（前置）顺序。 |
| [Multiply](../../aspose.page.xps.xpsmodel/xpsmatrix/multiply#multiply_3)(Matrix, MatrixOrder) | 将此矩阵乘以*matrix* 指定的矩阵，顺序由*matrixOrder指定*。 |
| [Multiply](../../aspose.page.xps.xpsmodel/xpsmatrix/multiply#multiply_1)(XpsMatrix, MatrixOrder) | 将此矩阵乘以*matrix* 指定的矩阵，顺序由*matrixOrder指定*。 |
| [Reset](../../aspose.page.xps.xpsmodel/xpsmatrix/reset)() | 将此矩阵重置为单位矩阵。 |
| [Rotate](../../aspose.page.xps.xpsmodel/xpsmatrix/rotate#rotate)(float) | 按默认（前置）顺序将*angle*顺时针旋转应用于此矩阵。 |
| [Rotate](../../aspose.page.xps.xpsmodel/xpsmatrix/rotate#rotate_1)(float, MatrixOrder) | 按*angle*顺时针旋转此矩阵，按顺序 由指定*matrixOrder*. |
| [RotateAround](../../aspose.page.xps.xpsmodel/xpsmatrix/rotatearound#rotatearound)(float, PointF) | 围绕*pivot* 应用顺时针旋转*angle*到这个矩阵默认（前置）订单。 |
| [RotateAround](../../aspose.page.xps.xpsmodel/xpsmatrix/rotatearound#rotatearound_1)(float, PointF, MatrixOrder) | 围绕*pivot* 应用顺时针旋转*angle*到这个矩阵*matrixOrder*指定的顺序。 |
| [Scale](../../aspose.page.xps.xpsmodel/xpsmatrix/scale#scale)(float, float) | 以默认（前置）顺序将指定的缩放向量（scaleX 和 scaleY）应用于此矩阵。 |
| [Scale](../../aspose.page.xps.xpsmodel/xpsmatrix/scale#scale_1)(float, float, MatrixOrder) | 按*matrixOrder*指定的顺序 将指定的缩放向量（scaleX 和 scaleY）应用于此矩阵。 |
| [Skew](../../aspose.page.xps.xpsmodel/xpsmatrix/skew)(double, double) | 将指定的倾斜变换应用于此矩阵。 |
| override [ToString](../../aspose.page.xps.xpsmodel/xpsmatrix/tostring)() | 返回此[`XpsMatrix`](../xpsmatrix)实例的字符串表示形式。 |
| [Transform](../../aspose.page.xps.xpsmodel/xpsmatrix/transform)(RectangleF) | 将此 Matrix 表示的仿射变换应用于指定的矩形。 |
| [TransformPoint](../../aspose.page.xps.xpsmodel/xpsmatrix/transformpoint)(PointF) | 将此 Matrix 表示的仿射变换应用于指定点。 |
| [TransformPoints](../../aspose.page.xps.xpsmodel/xpsmatrix/transformpoints#transformpoints)(PointF[]) | 将此 Matrix 表示的仿射变换应用于指定的点数组。 |
| [TransformPoints](../../aspose.page.xps.xpsmodel/xpsmatrix/transformpoints#transformpoints_1)(PointF[], int, int) | 将此矩阵表示的仿射变换应用于点数组的指定部分。 |
| [Translate](../../aspose.page.xps.xpsmodel/xpsmatrix/translate#translate)(float, float) | 将指定的平移向量应用于此矩阵。 |
| [Translate](../../aspose.page.xps.xpsmodel/xpsmatrix/translate#translate_1)(float, float, MatrixOrder) | 按照*matrixOrder*指定的顺序将指定的平移向量应用于此矩阵。 |
| static [Equals](../../aspose.page.xps.xpsmodel/xpsmatrix/equals)(XpsMatrix, XpsMatrix) | 实际实现。 |
| [operator ==](../../aspose.page.xps.xpsmodel/xpsmatrix/op_equality) | 实现运算符 ==。 |
| [operator !=](../../aspose.page.xps.xpsmodel/xpsmatrix/op_inequality) | 实现运算符 !=。 |

### 也可以看看

* class [XpsObject](../xpsobject)
* 命名空间 [Aspose.Page.XPS.XpsModel](../../aspose.page.xps.xpsmodel)
* 部件 [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->