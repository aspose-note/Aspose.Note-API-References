---
title: "DocumentFontsSubsystem.UsingDefaultFontFromStream"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "DocumentFontsSubsystem method. إنشاء نسخة جديدة من DocumentFontsSubsystem باستخدام خط من الدفق المحدد كافتراضي"
type: docs
weight: 50
url: /ar/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

أنشئ مثلاً جديداً من DocumentFontsSubsystem باستخدام خط من الدفق المحدد كافتراضي.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| defaultFontStream | Stream | الدفق الذي يحتوي على اسم الخط الافتراضي. |
| fontsSubstitutions | Dictionary`2 | استبدالات الخطوط. |

### قيمة الإرجاع

ال [`DocumentFontsSubsystem`](../).

## أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### انظر أيضًا

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


