---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note لمرجع NET API
description: DocumentFontsSubsystem طريقة. إنشاء مثيل DocumentFontsSubsystem جديد باستخدام خط من ملف محدد كملف افتراضي.
type: docs
weight: 40
url: /ar/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

إنشاء مثيل DocumentFontsSubsystem جديد باستخدام خط من ملف محدد كملف افتراضي.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | الملف الذي يحتوي على اسم الخط الافتراضي. |
| fontsSubstitutions | Dictionary`2 | بدائل الخطوط . |

### قيمة الإرجاع

ملف[`DocumentFontsSubsystem`](../) .

### أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من ملف.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### أنظر أيضا

* class [DocumentFontsSubsystem](../)
* مساحة الاسم [Aspose.Note.Fonts](../../documentfontssubsystem/)
* المجسم [Aspose.Note](../../../)


