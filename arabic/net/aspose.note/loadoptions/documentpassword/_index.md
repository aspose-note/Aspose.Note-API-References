---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note لمرجع NET API
description: LoadOptions ملكية. الحصول على أو تعيين كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حالة عدم كون المستند محميًا بكلمة مرور.
type: docs
weight: 20
url: /ar/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

الحصول على أو تعيين كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حالة عدم كون المستند محميًا بكلمة مرور.

```csharp
public string DocumentPassword { get; set; }
```

### أمثلة

يوضح كيفية عمل مستند مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

يوضح كيفية عمل دفتر ملاحظات مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### أنظر أيضا

* class [LoadOptions](../)
* مساحة الاسم [Aspose.Note](../../loadoptions/)
* المجسم [Aspose.Note](../../../)


