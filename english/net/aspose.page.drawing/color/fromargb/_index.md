---
title: Color.FromArgb
second_title: Aspose.Page for .NET API Reference
description: Color method. Creates a Color structure from a 32bit ARGB value
type: docs
weight: 1430
url: /net/aspose.page.drawing/color/fromargb/
---
## FromArgb(int) {#fromargb}

Creates a [`Color`](../) structure from a 32-bit ARGB value.

```csharp
public static Color FromArgb(int argb)
```

| Parameter | Type | Description |
| --- | --- | --- |
| argb | Int32 | A value specifying the 32-bit ARGB value. |

### Return Value

The [`Color`](../) structure that this method creates.

### See Also

* struct [Color](../)
* namespace [Aspose.Page.Drawing](../../color/)
* assembly [Aspose.Page](../../../)

---

## FromArgb(int, int, int, int) {#fromargb_3}

Creates a [`Color`](../) structure from the four ARGB component (alpha, red, green, and blue) values. Although this method allows a 32-bit value to be passed for each component, the value of each component is limited to 8 bits.

```csharp
public static Color FromArgb(int alpha, int red, int green, int blue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| alpha | Int32 | The alpha component. Valid values are 0 through 255. |
| red | Int32 | The red component. Valid values are 0 through 255. |
| green | Int32 | The green component. Valid values are 0 through 255. |
| blue | Int32 | The blue component. Valid values are 0 through 255. |

### Return Value

The [`Color`](../) that this method creates.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *alpha*, *red*, *green*, or *blue* is less than 0 or greater than 255. |

### See Also

* struct [Color](../)
* namespace [Aspose.Page.Drawing](../../color/)
* assembly [Aspose.Page](../../../)

---

## FromArgb(int, Color) {#fromargb_1}

Creates a [`Color`](../) structure from the specified [`Color`](../) structure, but with the new specified alpha value. Although this method allows a 32-bit value to be passed for the alpha value, the value is limited to 8 bits.

```csharp
public static Color FromArgb(int alpha, Color baseColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| alpha | Int32 | The alpha value for the new [`Color`](../). Valid values are 0 through 255. |
| baseColor | Color | The [`Color`](../) from which to create the new [`Color`](../). |

### Return Value

The [`Color`](../) that this method creates.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *alpha* is less than 0 or greater than 255. |

### See Also

* struct [Color](../)
* namespace [Aspose.Page.Drawing](../../color/)
* assembly [Aspose.Page](../../../)

---

## FromArgb(int, int, int) {#fromargb_2}

Creates a [`Color`](../) structure from the specified 8-bit color values (red, green, and blue). The alpha value is implicitly 255 (fully opaque). Although this method allows a 32-bit value to be passed for each color component, the value of each component is limited to 8 bits.

```csharp
public static Color FromArgb(int red, int green, int blue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| red | Int32 | The red component value for the new [`Color`](../). Valid values are 0 through 255. |
| green | Int32 | The green component value for the new [`Color`](../). Valid values are 0 through 255. |
| blue | Int32 | The blue component value for the new [`Color`](../). Valid values are 0 through 255. |

### Return Value

The [`Color`](../) that this method creates.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *red*, *green*, or *blue* is less than 0 or greater than 255. |

### See Also

* struct [Color](../)
* namespace [Aspose.Page.Drawing](../../color/)
* assembly [Aspose.Page](../../../)


