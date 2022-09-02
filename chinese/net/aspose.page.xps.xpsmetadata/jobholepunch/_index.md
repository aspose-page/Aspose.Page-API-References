---
title: JobHolePunch
second_title: Aspose.Page for .NET API 参考
description: 描述输出的打孔特性所有文件都打孔在一起 JobHolePunch./jobholepunch和DocumentHolePunch./documentholepunch关键字是互斥的 不应在 PrintTicket 或 Print Capabilities 文档中同时指定两者 https//docs.microsoft.com/enus/windows/win32/printdocs/jobholepunch
type: docs
weight: 1290
url: /zh/net/aspose.page.xps.xpsmetadata/jobholepunch/
---
## JobHolePunch class

描述输出的打孔特性。所有文件都打孔在一起。 [`JobHolePunch`](../jobholepunch)和[`DocumentHolePunch`](../documentholepunch)关键字是互斥的。 不应在 PrintTicket 或 Print Capabilities 文档中同时指定两者。 https://docs.microsoft.com/en-us/windows/win32/printdocs/jobholepunch

```csharp
public sealed class JobHolePunch : HolePunch, IJobPrintTicketItem
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [JobHolePunch](jobholepunch)(params HolePunchOption[]) | 创建一个新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Name](../../aspose.page.xps.xpsmetadata/printticketelement/name) { get; } | 获取元素名称。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.page.xps.xpsmetadata/feature/add)(params IFeatureItem[]) | 将项目列表添加到此功能项目列表的末尾。 每一个都必须是一个[`Feature`](../feature)， 一个[`Option`](../option)或一个[`Property`](../property)实例. |

### 也可以看看

* class [HolePunch](../holepunch)
* interface [IJobPrintTicketItem](../ijobprintticketitem)
* 命名空间 [Aspose.Page.XPS.XpsMetadata](../../aspose.page.xps.xpsmetadata)
* 部件 [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->