---
title: "LoadOptions.DocumentPassword"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية LoadOptions. يحصل أو يحدد كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حال عدم حماية المستند بكلمة مرور"
type: docs
weight: 20
url: /ar/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

يحصل أو يضبط كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حال عدم حماية المستند بكلمة مرور.

```csharp
public string DocumentPassword { get; set; }
```

## أمثلة

يعرض كيفية التعامل مع مستند مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

يوضح كيفية التعامل مع دفتر مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Note](../../loadoptions/)
* assembly [Aspose.Note](../../../)


