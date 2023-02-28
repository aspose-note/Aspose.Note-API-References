---
title: NumberList.Format
second_title: Aspose.Note for .NET API Referansı
description: NumberList mülk. Satır başlığının biçimini alır veya ayarlar. Madde işaretli listeler için madde işareti sembolünü temsil eder.
type: docs
weight: 50
url: /tr/net/aspose.note/numberlist/format/
---
## NumberList.Format property

Satır başlığının biçimini alır veya ayarlar. Madde işaretli listeler için madde işareti sembolünü temsil eder.

```csharp
public string Format { get; set; }
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


