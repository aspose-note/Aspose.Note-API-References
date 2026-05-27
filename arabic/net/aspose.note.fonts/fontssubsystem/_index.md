---
title: "الفئة FontsSubsystem"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Fonts.FontsSubsystem. الفئة الأساسية التي تنفّذ واجهة Aspose.Note.Fonts.IFontsSubsystem. توفر وظائف للخط الافتراضي واستبدالات الخطوط. قم بتجاوز الدالة المحمية Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily في فئة مشتقة لتنفيذ المنطق الخاص باسترجاع كائن FontFamily."
type: docs
weight: 110
url: /ar/net/aspose.note.fonts/fontssubsystem/
---
## FontsSubsystem class

الفئة الأساسية التي تنفذ واجهة Aspose.Note.Fonts.IFontsSubsystem. توفر وظائف للخط الافتراضي واستبدالات الخط. قم بتجاوز الدالة المحمية Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily في فئة مشتقة لتنفيذ منطق استرجاع كائن FontFamily.

```csharp
public abstract class FontsSubsystem : IFontsSubsystem
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | يحصل أو يعيّن الخط الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont)(Stream) | أضف الخط. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_2)(string) | أضف الخط. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_1)(Stream, string) | أضف الخط. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | يضيف استبدال الخط. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | يحصل على عائلة الخط. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | يقوم بتحميل جميع خطوط TrueType من المجلد المحدد إلى المجموعة الداخلية. |

### انظر أيضًا

* interface [IFontsSubsystem](../ifontssubsystem/)
* namespace [Aspose.Note.Fonts](../../aspose.note.fonts/)
* assembly [Aspose.Note](../../)


