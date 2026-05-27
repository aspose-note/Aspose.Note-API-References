---
title: "OneSaveOptions.DocumentPassword"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "OneSaveOptions property. يحصل أو يعيّن كلمة مرور لتشفير محتوى المستند"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

يحصل أو يعيّن كلمة مرور لتشفير محتوى المستند.

```csharp
public string DocumentPassword { get; set; }
```

## أمثلة

يعرض كيفية حفظ المستند مع التشفير.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### انظر أيضًا

* class [OneSaveOptions](../)
* namespace [Aspose.Note.Saving](../../onesaveoptions/)
* assembly [Aspose.Note](../../../)


