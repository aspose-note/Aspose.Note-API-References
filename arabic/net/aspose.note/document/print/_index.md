---
title: "Document.Print"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Document. تطبع المستند باستخدام الطابعة الافتراضية"
type: docs
weight: 130
url: /ar/net/aspose.note/document/print/
---
## Print() {#print}

يطبع المستند باستخدام الطابعة الافتراضية.

```csharp
public void Print()
```

## أمثلة

يوضح كيفية إرسال المستند إلى طابعة باستخدام مربع حوار Windows القياسي مع الخيارات الافتراضية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

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

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

يطبع المستند باستخدام الطابعة الافتراضية.

```csharp
public void Print(PrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | PrintOptions | خيارات تُستخدم لطباعة مستند. يمكن أن تكون فارغة. |

### انظر أيضًا

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


