---
title: NumberList.FontSize
second_title: Aspose.Note .NET API संदर्भ के लिए
description: NumberList संपत्त. फ़न्ट आकर प्रप्त य सेट करत है
type: docs
weight: 40
url: /hi/net/aspose.note/numberlist/fontsize/
---
## NumberList.FontSize property

फ़ॉन्ट आकार प्राप्त या सेट करता है।

```csharp
public int FontSize { get; set; }
```

### उदाहरण

दिखाता है कि सूची के स्वरूपण के बारे में जानकारी कैसे प्राप्त करें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// रूपरेखा तत्व के संग्रह नोड्स को पुनः प्राप्त करें
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// प्रत्येक नोड के माध्यम से दोहराएं
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // फ़ॉन्ट नाम पुनर्प्राप्त करें
        Console.WriteLine("Font Name: " + list.Font);

        // फ़ॉन्ट लंबाई पुनर्प्राप्त करें
        Console.WriteLine("Font Length: " + list.Font.Length);

        // फ़ॉन्ट आकार पुनर्प्राप्त करें
        Console.WriteLine("Font Size: " + list.FontSize);

        // फ़ॉन्ट रंग पुनर्प्राप्त करें
        Console.WriteLine("Font Color: " + list.FontColor);

        // स्वरूप प्राप्त करें
        Console.WriteLine("Font format: " + list.Format);

        // बोल्ड चेक करें
        Console.WriteLine("Is bold: " + list.IsBold);

        // इटैलिक चेक करें
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### यह सभी देखें

* class [NumberList](../)
* नाम स्थान [Aspose.Note](../../numberlist/)
* सभा [Aspose.Note](../../../)


