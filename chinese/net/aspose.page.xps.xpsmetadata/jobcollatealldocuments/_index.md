---
title: JobCollateAllDocuments
second_title: Aspose.Page for .NET API 参考
description: 描述输出的整理特性每个单独作业中的所有文档都经过整理 DocumentCollate./documentcollate和JobCollateAllDocuments./jobcollatealldocuments是互斥的 是否实现这两个关键字或仅一个关键字的行为和实现由驱动程序决定 https//docs.microsoft.com/enus/windows/win32/printdocs/jobcollatealldocuments
type: docs
weight: 1140
url: /zh/net/aspose.page.xps.xpsmetadata/jobcollatealldocuments/
---
## JobCollateAllDocuments class

描述输出的整理特性。每个单独作业中的所有文档都经过整理。 [`DocumentCollate`](../documentcollate)和[`JobCollateAllDocuments`](../jobcollatealldocuments)是互斥的。 是否实现这两个关键字或仅一个关键字的行为和实现由驱动程序决定。 https://docs.microsoft.com/en-us/windows/win32/printdocs/jobcollatealldocuments

```csharp
public sealed class JobCollateAllDocuments : Collate, IJobPrintTicketItem
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [JobCollateAllDocuments](jobcollatealldocuments)(params CollateOption[]) | 创建一个新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Name](../../aspose.page.xps.xpsmetadata/printticketelement/name) { get; } | 获取元素名称。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.page.xps.xpsmetadata/feature/add)(params IFeatureItem[]) | 将项目列表添加到此功能项目列表的末尾。 每一个都必须是一个[`Feature`](../feature)， 一个[`Option`](../option)或一个[`Property`](../property)实例. |

### 也可以看看

* class [Collate](../collate)
* interface [IJobPrintTicketItem](../ijobprintticketitem)
* 命名空间 [Aspose.Page.XPS.XpsMetadata](../../aspose.page.xps.xpsmetadata)
* 部件 [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->