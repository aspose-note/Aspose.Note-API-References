---
title: "DocumentFontsSubsystem.UsingDefaultFontFromFile"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "DocumentFontsSubsystem method. إنشاء نسخة جديدة من DocumentFontsSubsystem باستخدام خط من الملف المحدد كافتراضي"
type: docs
weight: 40
url: /ar/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

أنشئ مثلاً جديداً من DocumentFontsSubsystem باستخدام خط من الملف المحدد كافتراضي.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | الملف الذي يحتوي على اسم الخط الافتراضي. |
| fontsSubstitutions | Dictionary`2 | استبدالات الخطوط. |

### قيمة الإرجاع

ال [`DocumentFontsSubsystem`](../).

## أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من ملف.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### انظر أيضًا

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


