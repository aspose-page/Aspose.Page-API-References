---
title: DrFont
second_title: Aspose.Page for .NET API Referansı
description: GDI Font yerine bu sınıfı kullanın
type: docs
weight: 160
url: /tr/net/aspose.page.font/drfont/
---
## DrFont class

GDI+ Font yerine bu sınıfı kullanın

```csharp
public class DrFont
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AscentLis](../../aspose.page.font/drfont/ascentlis) { get; } | Bu yazı tipinin (lis) hücre yükselişi. Bu, hücrenin tepesinden hücre taban çizgisine dikey bir mesafedir. |
| [AscentPoints](../../aspose.page.font/drfont/ascentpoints) { get; } | Hücre çıkışını puan olarak döndürür. |
| [CellHeightLis](../../aspose.page.font/drfont/cellheightlis) { get; } | Bu yazı tipinin (lis) hücre yüksekliğini döndürür. Bu, şunun için bir kısayoldur:[`AscentLis`](./ascentlis) +[`DescentLis`](./descentlis) . |
| [CellHeightPoints](../../aspose.page.font/drfont/cellheightpoints) { get; } | için kısayol[`AscentPoints`](./ascentpoints) +[`DescentPoints`](./descentpoints) . |
| [DescentLis](../../aspose.page.font/drfont/descentlis) { get; } | Bu yazı tipinin hücre inişi (lis). Bu, hücrenin altından hücre taban çizgisine kadar olan dikey mesafedir. |
| [DescentPoints](../../aspose.page.font/drfont/descentpoints) { get; } | Nokta olarak hücre inişini döndürür. |
| [FamilyName](../../aspose.page.font/drfont/familyname) { get; } | Bu yazı tipinin adını alır. |
| [IsBold](../../aspose.page.font/drfont/isbold) { get; } | Bu örneğin kalın olup olmadığını gösteren bir değer alır. |
| [IsItalic](../../aspose.page.font/drfont/isitalic) { get; } | Bu örneğin italik olup olmadığını gösteren bir değer alır. |
| [LeadingLis](../../aspose.page.font/drfont/leadinglis) { get; } | Bu yazı tipinin (lis) başını döndürür. Bu, şunun için bir kısayoldur:[`LineSpacingLis`](./linespacinglis) -[`CellHeightLis`](./cellheightlis) . |
| [LeadingPoints](../../aspose.page.font/drfont/leadingpoints) { get; } | Bu yazı tipinin (lis) başını döndürür. Bu, şunun için bir kısayoldur:[`LineSpacingLis`](./linespacinglis) -[`CellHeightLis`](./cellheightlis) . |
| [LineSpacingLis](../../aspose.page.font/drfont/linespacinglis) { get; } | Bu yazı tipinin (lis) hücre aralığını döndürür. Bu, iki glifin taban çizgileri arasındaki dikey mesafedir. |
| [LineSpacingPoints](../../aspose.page.font/drfont/linespacingpoints) { get; } | Bu yazı tipinin hücre aralığını verir (nokta). Bu, iki glifin taban çizgileri arasındaki dikey mesafedir. |
| [SizePoints](../../aspose.page.font/drfont/sizepoints) { get; set; } | Bu yazı tipinin boyutunu alır (puan). |
| [SmallCapsScaleFactor](../../aspose.page.font/drfont/smallcapsscalefactor) { get; } | SmallCaps ölçek faktörünü alır. |
| [Style](../../aspose.page.font/drfont/style) { get; } | Bu yazı tipinin stilini alır. |
| [StyleEx](../../aspose.page.font/drfont/styleex) { get; set; } | Bu özellik, yazı tipinin stili hakkında ek bilgiler içerir |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Equals](../../aspose.page.font/drfont/equals)(object) | BelirtilenObject , bu örneğe eşittir. |
| [GetCharWidthLis](../../aspose.page.font/drfont/getcharwidthlis)(char) | lis karakter genişliğini alır. |
| [GetCharWidthPoints](../../aspose.page.font/drfont/getcharwidthpoints)(char) | Karakterin genişliğini verir (puan). |
| override [GetHashCode](../../aspose.page.font/drfont/gethashcode)() | Bu örnek için bir karma kod döndürür. |
| [GetTextSizePoints](../../aspose.page.font/drfont/gettextsizepoints)(string) | Metnin nokta cinsinden ölçüm metin kutusunu döndürür. |
| [GetTextWidthLis](../../aspose.page.font/drfont/gettextwidthlis)(string) | lis. metin genişliğini alır |
| [GetTextWidthPoints](../../aspose.page.font/drfont/gettextwidthpoints#gettextwidthpoints)(string) | Metin genişliği noktalarını alır. |
| [GetTextWidthPoints](../../aspose.page.font/drfont/gettextwidthpoints#gettextwidthpoints_1)(string, int, int) | Metin genişliği noktalarını alır. |
| [Replace](../../aspose.page.font/drfont/replace)(DrFont) | Yazı tipi içeriğini değiştir |
| static [IsPoorlyRenderedByGdiPlus](../../aspose.page.font/drfont/ispoorlyrenderedbygdiplus)(string) | "Microsoft Sans Serif" yazı tipi için True değerini döndürür. Bu, GDI+ tarafından kötü bir şekilde işlenmiştir. Test286 ve Gemini-6959'a bakın. |

### Ayrıca bakınız

* ad alanı [Aspose.Page.Font](../../aspose.page.font)
* toplantı [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->