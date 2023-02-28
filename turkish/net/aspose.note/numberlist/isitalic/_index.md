---
title: NumberList.IsItalic
second_title: Aspose.Note for .NET API Referansı
description: NumberList mülk. Metin stilinin italik olup olmadığını gösteren bir değer alır veya ayarlar.
type: docs
weight: 70
url: /tr/net/aspose.note/numberlist/isitalic/
---
## NumberList.IsItalic property

Metin stilinin italik olup olmadığını gösteren bir değer alır veya ayarlar.

```csharp
public bool IsItalic { get; set; }
```

### Örnekler

Listenin biçimlendirmesiyle ilgili bilgilerin nasıl alınacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Anahat öğesinin toplama düğümlerini alın
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Her düğümü yinele
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Yazı tipi adını al
        Console.WriteLine("Font Name: " + list.Font);

        // yazı tipi uzunluğunu al
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Yazı tipi boyutunu al
        Console.WriteLine("Font Size: " + list.FontSize);

        // yazı tipi rengini al
        Console.WriteLine("Font Color: " + list.FontColor);

        // formatı al
        Console.WriteLine("Font format: " + list.Format);

        // kalın işaretle
        Console.WriteLine("Is bold: " + list.IsBold);

        // italik kontrol et
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Ayrıca bakınız

* class [NumberList](../)
* ad alanı [Aspose.Note](../../numberlist/)
* toplantı [Aspose.Note](../../../)


