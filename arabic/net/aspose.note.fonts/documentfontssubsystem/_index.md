---
title: "الفئة DocumentFontsSubsystem"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Fonts.DocumentFontsSubsystem. تنفيذ بسيط لـ Aspose.Note.Fonts.FontsSubsystem. يسترجع كائن FontFamily من نظام التشغيل"
type: docs
weight: 100
url: /ar/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

تنفيذ بسيط لـ Aspose.Note.Fonts.FontsSubsystem. يسترجع كائن FontFamily من نظام التشغيل.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | يُنشئ مثلاً جديداً للفئة `DocumentFontsSubsystem`. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | يُنشئ مثلاً جديداً للفئة `DocumentFontsSubsystem`. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | يُنشئ مثلاً جديداً للفئة `DocumentFontsSubsystem`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | يحصل أو يعيّن المثيل الافتراضي الثابت. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | يحصل أو يعيّن الخط الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | أنشئ مثلاً جديداً من DocumentFontsSubsystem باستخدام اسم الخط الافتراضي المحدد. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | أنشئ مثلاً جديداً من DocumentFontsSubsystem باستخدام خط من الملف المحدد كافتراضي. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | أنشئ مثلاً جديداً من DocumentFontsSubsystem باستخدام خط من الدفق المحدد كافتراضي. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | أضف الخط. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | أضف الخط. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | أضف الخط. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | يضيف استبدال الخط. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | يحصل على عائلة الخط. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | يقوم بتحميل جميع خطوط TrueType من المجلد المحدد إلى المجموعة الداخلية. |

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

* class [FontsSubsystem](../fontssubsystem/)
* namespace [Aspose.Note.Fonts](../../aspose.note.fonts/)
* assembly [Aspose.Note](../../)


