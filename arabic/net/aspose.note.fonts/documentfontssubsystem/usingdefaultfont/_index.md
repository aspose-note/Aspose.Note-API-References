---
title: "DocumentFontsSubsystem.UsingDefaultFont"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "طريقة DocumentFontsSubsystem. إنشاء مثيل جديد من DocumentFontsSubsystem باستخدام اسم الخط الافتراضي المحدد"
type: docs
weight: 30
url: /ar/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

أنشئ مثيلًا جديدًا من DocumentFontsSubsystem باستخدام اسم الخط الافتراضي المحدد.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| defaultFontName | String | اسم الخط الافتراضي. |
| fontsSubstitutions | Dictionary`2 | استبدالات الخطوط. |

### قيمة الإرجاع

الـ [`DocumentFontsSubsystem`](../).

## أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي المحدد.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### انظر أيضًا

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


