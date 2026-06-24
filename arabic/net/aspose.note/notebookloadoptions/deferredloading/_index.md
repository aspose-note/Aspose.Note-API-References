---
title: "NotebookLoadOptions.DeferredLoading"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية NotebookLoadOptions. يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال صراحةً لاحقًا"
type: docs
weight: 20
url: /ar/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية صراحةً لاحقًا.

```csharp
public bool DeferredLoading { get; set; }
```

## ملاحظات

القيمة الافتراضية هي `false`، لذا سيتم تحميل المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أنه يجب على المستخدم استدعاء [`LoadChildDocument`](../../notebook/loadchilddocument/) أو  لكل عقدة فرعية في الدفتر بعد تحميل الدفتر نفسه. إذا كانت القيمة `true`، سيتم تجاهل خيار [`InstantLoading`](../instantloading/). إذا كان الدفتر يُحمَّل من تدفق، تكون القيمة دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

## أمثلة

يظهر كيفية دفتر مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### انظر أيضًا

* class [NotebookLoadOptions](../)
* namespace [Aspose.Note](../../notebookloadoptions/)
* assembly [Aspose.Note](../../../)


