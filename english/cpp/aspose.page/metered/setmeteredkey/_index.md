---
title: Aspose::Page::Metered::SetMeteredKey method
linktitle: SetMeteredKey
second_title: Aspose.Page for C++
description: 'Aspose::Page::Metered::SetMeteredKey method. Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again in C++.'
type: docs
weight: 200
url: /cpp/aspose.page/metered/setmeteredkey/
---
## Metered::SetMeteredKey method


Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

```cpp
void Aspose::Page::Metered::SetMeteredKey(System::String publicKey, System::String privateKey)
```


| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | System::String | public key |
| privateKey | System::String | private key |

## See Also

* Class [String](../../../system/string/)
* Class [Metered](../)
* Namespace [Aspose::Page](../../)
* Library [Aspose.Page for C++](../../../)
