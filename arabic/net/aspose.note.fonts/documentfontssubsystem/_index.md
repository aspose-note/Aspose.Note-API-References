---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Fonts.DocumentFontsSubsystem فصل. تنفيذ بسيط لـ Aspose.Note.Fonts.FontsSubsystem. يستردFontFamily كائن من OS.
type: docs
weight: 100
url: /ar/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

تنفيذ بسيط لـ Aspose.Note.Fonts.FontsSubsystem. يستردFontFamily كائن من OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | يقوم بتهيئة مثيل جديد لملف`DocumentFontsSubsystem` فئة . |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | يقوم بتهيئة مثيل جديد لملف`DocumentFontsSubsystem` فئة . |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | يقوم بتهيئة مثيل جديد لملف`DocumentFontsSubsystem` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | الحصول على المثيل الافتراضي الثابت أو تعيينه. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | الحصول على الخط الافتراضي أو تعيينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | إنشاء مثيل DocumentFontsSubsystem جديد باستخدام اسم الخط الافتراضي المحدد. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | إنشاء مثيل DocumentFontsSubsystem جديد باستخدام خط من ملف محدد كملف افتراضي. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | إنشاء مثيل DocumentFontsSubsystem جديد باستخدام خط من دفق محدد كافتراضي. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | أضف الخط. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | أضف الخط. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | أضف الخط. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | إضافة استبدال الخط . |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | يحصل على عائلة الخطوط . |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | يتم تحميل كافة خطوط TrueType من المجلد المحدد إلى المجموعة الداخلية. |

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

* class [FontsSubsystem](../fontssubsystem/)
* مساحة الاسم [Aspose.Note.Fonts](../../aspose.note.fonts/)
* المجسم [Aspose.Note](../../)


