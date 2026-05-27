---
title: "Page.GetChildNodes"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Page. احصل على جميع العقد الفرعية للصفحة حسب نوع العقدة"
type: docs
weight: 150
url: /ar/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

احصل على جميع العقد الفرعية للصفحة حسب نوع العقدة.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| معامل | الوصف |
| --- | --- |
| T1 | نوع العناصر في القائمة المعادة. |

### قيمة الإرجاع

قائمة من العقد الفرعية.

## أمثلة

يوضح كيفية الحصول على كل النص من المستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// استرجاع النص
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// طباعة النص على شاشة الإخراج
Console.WriteLine(text);
```

يوضح كيفية الحصول على كل النص من الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على قائمة بعقد الصفحة
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // استرجاع النص
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // طباعة النص على شاشة الإخراج
    Console.WriteLine(text);
}
```

يوضح كيفية المرور عبر جميع الصفحات وإجراء استبدال في النص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عقد RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // استبدال نص الشكل
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// احفظ بأي تنسيق ملف مدعوم
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يوضح كيفية المرور عبر نص الصفحة وإجراء استبدال.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// احصل على جميع عقد RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // استبدال نص الشكل
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// احفظ بأي تنسيق ملف مدعوم
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### انظر أيضًا

* interface [INode](../../inode/)
* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


