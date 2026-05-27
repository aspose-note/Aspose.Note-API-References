---
title: "NumberList.IsBold"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية NumberList. تحصل أو تعين قيمة تشير إلى ما إذا كان نمط النص غامقًا"
type: docs
weight: 60
url: /ar/net/aspose.note/numberlist/isbold/
---
## NumberList.IsBold property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص غامقًا.

```csharp
public bool IsBold { get; set; }
```

## أمثلة

يوضح كيفية استرجاع معلومات حول تنسيق القائمة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// استرجاع مجموعة العقد لعنصر المخطط.
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// تكرار عبر كل عقدة
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // استرجاع اسم الخط
        Console.WriteLine("Font Name: " + list.Font);

        // استرجاع طول الخط
        Console.WriteLine("Font Length: " + list.Font.Length);

        // استرجاع حجم الخط
        Console.WriteLine("Font Size: " + list.FontSize);

        // استرجاع لون الخط
        Console.WriteLine("Font Color: " + list.FontColor);

        // استرجاع التنسيق
        Console.WriteLine("Font format: " + list.Format);

        // التحقق من الغامق
        Console.WriteLine("Is bold: " + list.IsBold);

        // التحقق من المائل
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### انظر أيضًا

* class [NumberList](../)
* namespace [Aspose.Note](../../numberlist/)
* assembly [Aspose.Note](../../../)


