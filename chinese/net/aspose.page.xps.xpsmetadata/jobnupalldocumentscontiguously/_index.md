---
title: JobNUpAllDocumentsContiguously
second_title: Aspose.Page for .NET API 参考
description: 将多个逻辑页面的输出描述到单个物理表 job 中的所有文档都是连续编译的JobNUpAllDocumentsContiguously./jobnupalldocumentscontiguously和DocumentNUp./documentnup 是互斥的由驱动程序来确定这些关键字之间的约束处理 https//docs.microsoft.com/enus/windows/win32/printdocs/jobnupalldocumentscontiguously
type: docs
weight: 1320
url: /zh/net/aspose.page.xps.xpsmetadata/jobnupalldocumentscontiguously/
---
## JobNUpAllDocumentsContiguously class

将多个逻辑页面的输出描述到单个物理表。 job 中的所有文档都是连续编译的。[`JobNUpAllDocumentsContiguously`](../jobnupalldocumentscontiguously)和[`DocumentNUp`](../documentnup) 是互斥的。由驱动程序来确定这些关键字之间的约束处理。 https://docs.microsoft.com/en-us/windows/win32/printdocs/jobnupalldocumentscontiguously

```csharp
public sealed class JobNUpAllDocumentsContiguously : NUp, IJobPrintTicketItem
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [JobNUpAllDocumentsContiguously](jobnupalldocumentscontiguously)(params INUpItem[]) | 创建一个新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Name](../../aspose.page.xps.xpsmetadata/printticketelement/name) { get; } | 获取元素名称。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.page.xps.xpsmetadata/feature/add)(params IFeatureItem[]) | 将项目列表添加到此功能项目列表的末尾。 每一个都必须是一个[`Feature`](../feature)， 一个[`Option`](../option)或一个[`Property`](../property)实例. |
| [AddPagesPerSheetOption](../../aspose.page.xps.xpsmetadata/jobnupalldocumentscontiguously/addpagespersheetoption)(int) | 添加和选项得分属性值。 指定每个物理表的逻辑页数。 |

### 也可以看看

* class [NUp](../nup)
* interface [IJobPrintTicketItem](../ijobprintticketitem)
* 命名空间 [Aspose.Page.XPS.XpsMetadata](../../aspose.page.xps.xpsmetadata)
* 部件 [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->