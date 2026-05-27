---
title: "الفئة OneSaveOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.OneSaveOptions. يسمح بتحديد خيارات إضافية عند حفظ المستند إلى تنسيق OneNote"
type: docs
weight: 890
url: /ar/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ المستند إلى تنسيق OneNote.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | يحصل أو يعيّن كلمة مرور لتشفير محتوى المستند. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | يحصل أو يضبط إعدادات الخط التي سيتم استخدامها أثناء الحفظ |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها. القيمة الافتراضية هي MaxValue مما يعني أنه سيتم عرض جميع صفحات المستند. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | يحصل أو يضبط فهرس الصفحة الأولى التي سيتم حفظها. القيمة الافتراضية هي 0. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | يحصل على الصيغة التي يُحفظ بها المستند. |

## أمثلة

يعرض كيفية حفظ المستند مع التشفير.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

يعرض كيفية حفظ مستند باستخدام OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### انظر أيضًا

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


