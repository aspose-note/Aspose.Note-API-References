---
title: NumberList.FontSize
second_title: Aspose.Note لمرجع NET API
description: NumberList ملكية. الحصول على حجم الخط أو تحديده.
type: docs
weight: 40
url: /ar/net/aspose.note/numberlist/fontsize/
---
## NumberList.FontSize property

الحصول على حجم الخط أو تحديده.

```csharp
public int FontSize { get; set; }
```

### أمثلة

يوضح كيفية استرداد المعلومات حول تنسيق القائمة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// استرداد عقد مجموعة لعنصر المخطط التفصيلي
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// كرر خلال كل عقدة
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // استرداد اسم الخط
        Console.WriteLine("Font Name: " + list.Font);

        // استرداد طول الخط
        Console.WriteLine("Font Length: " + list.Font.Length);

        // استرداد حجم الخط
        Console.WriteLine("Font Size: " + list.FontSize);

        // استرداد لون الخط
        Console.WriteLine("Font Color: " + list.FontColor);

        // استرداد التنسيق
        Console.WriteLine("Font format: " + list.Format);

        // تحقق بخط عريض
        Console.WriteLine("Is bold: " + list.IsBold);

        // تحقق من الخط المائل
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### أنظر أيضا

* class [NumberList](../)
* مساحة الاسم [Aspose.Note](../../numberlist/)
* المجسم [Aspose.Note](../../../)


