﻿---
title: Metered class
second_title: Aspose.Page for Python via .NET API References
description: 
type: docs
weight: 110
url: /python-net/aspose.page/metered/
is_root: false
---

## Metered class

Provides methods to set metered key.



The Metered type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/page/python-net/aspose.page/metered/__init__/#) | Initializes a new instance of this class. |


### Methods
| Method | Description |
| :- | :- |
| [set_metered_key](/page/python-net/aspose.page/metered/set_metered_key/#str-str) | Sets metered public and private key.<br/>If you purchase metered license, when start application, this API should be called, normally, this is enough. <br/>However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, <br/>to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again. |
| [get_consumption_quantity](/page/python-net/aspose.page/metered/get_consumption_quantity/#) | Gets consumption file size |
| [get_consumption_credit](/page/python-net/aspose.page/metered/get_consumption_credit/#) | Gets consumption credit |



### Example 


In this example, an attempt will be made to set metered public and private key


```python
from aspose.page import Metered

metered = Metered()
metered.set_metered_key("PublicKey", "PrivateKey")

```

### See Also
* module [`aspose.page`](..)
