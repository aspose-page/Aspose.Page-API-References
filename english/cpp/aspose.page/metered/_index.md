---
title: Aspose::Page::Metered class
linktitle: Metered
second_title: Aspose.Page for C++
description: 'Aspose::Page::Metered class. Provides methods to set metered key in C++.'
type: docs
weight: 1300
url: /cpp/aspose.page/metered/
---
## Metered class


Provides methods to set metered key.

```cpp
class Metered : public System::Object
```

## Methods

| Method | Description |
| --- | --- |
| static [GetConsumptionCredit](./getconsumptioncredit/)() | Gets consumption credit. |
| static [GetConsumptionQuantity](./getconsumptionquantity/)() | Gets consumption file size. |
| [Metered](./metered/)() | Initializes a new instance of this class. |
| [SetMeteredKey](./setmeteredkey/)(System::String, System::String) | Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again. |
## See Also

* Class [Object](../../system/object/)
* Namespace [Aspose::Page](../)
* Library [Aspose.Page for C++](../../)
