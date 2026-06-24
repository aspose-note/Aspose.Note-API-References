---
title: "NumberList.IsItalic"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية NumberList. يحصل أو يعيّن قيمة تشير إلى ما إذا كان نمط النص مائلًا"
type: docs
weight: 70
url: /ar/net/aspose.note/numberlist/isitalic/
---
## NumberList.IsItalic property

يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مائلًا.

```csharp
public bool IsItalic { get; set; }
```

## أمثلة

يعرض كيفية استرجاع معلومات تنسيق القائمة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// استرجاع مجموعة العقد لعنصر المخطط
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

        // تحقق من الغامق
        Console.WriteLine("Is bold: " + list.IsBold);

        // تحقق من المائل
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### انظر أيضًا

* class [NumberList](../)
* namespace [Aspose.Note](../../numberlist/)
* assembly [Aspose.Note](../../../)


