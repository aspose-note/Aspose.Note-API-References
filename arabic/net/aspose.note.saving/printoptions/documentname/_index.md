---
title: "PrintOptions.DocumentName"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "PrintOptions property. يحصل أو يعيّن اسم المستند لعرضه على سبيل المثال في مربع حوار حالة الطباعة أو طابور الطابعة أثناء طباعة المستند"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

يحصل أو يعيّن اسم المستند للعرض (على سبيل المثال، في مربع حوار حالة الطباعة أو في طابور الطابعة) أثناء طباعة المستند.

```csharp
public string DocumentName { get; set; }
```

## أمثلة

يظهر كيفية إرسال المستند إلى طابعة باستخدام مربع حوار Windows القياسي مع الخيارات المحددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### انظر أيضًا

* class [PrintOptions](../)
* namespace [Aspose.Note.Saving](../../printoptions/)
* assembly [Aspose.Note](../../../)


