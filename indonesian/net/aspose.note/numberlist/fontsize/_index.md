---
title: NumberList.FontSize
second_title: Aspose.Note untuk Referensi .NET API
description: NumberList Properti. Mendapat atau mengatur ukuran font.
type: docs
weight: 40
url: /id/net/aspose.note/numberlist/fontsize/
---
## NumberList.FontSize property

Mendapat atau mengatur ukuran font.

```csharp
public int FontSize { get; set; }
```

### Contoh

Memperlihatkan cara mengambil informasi tentang pemformatan daftar.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Ambil kumpulan simpul dari elemen kerangka
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterasi melalui setiap node
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Ambil nama font
        Console.WriteLine("Font Name: " + list.Font);

        // Ambil panjang font
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Ambil ukuran font
        Console.WriteLine("Font Size: " + list.FontSize);

        // Ambil warna font
        Console.WriteLine("Font Color: " + list.FontColor);

        // Ambil format
        Console.WriteLine("Font format: " + list.Format);

        // Centang tebal
        Console.WriteLine("Is bold: " + list.IsBold);

        // Centang miring
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Lihat juga

* class [NumberList](../)
* ruang nama [Aspose.Note](../../numberlist/)
* perakitan [Aspose.Note](../../../)


