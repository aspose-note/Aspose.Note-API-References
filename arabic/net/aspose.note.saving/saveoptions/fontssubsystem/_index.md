---
title: SaveOptions.FontsSubsystem
second_title: Aspose.Note لمرجع NET API
description: SaveOptions ملكية. الحصول على أو تعيين إعدادات الخط لاستخدامها أثناء الحفظ
type: docs
weight: 10
url: /ar/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

الحصول على أو تعيين إعدادات الخط لاستخدامها أثناء الحفظ

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

### أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي المحدد.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

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

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الخط الافتراضي من التدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### أنظر أيضا

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../saveoptions/)
* المجسم [Aspose.Note](../../../)


