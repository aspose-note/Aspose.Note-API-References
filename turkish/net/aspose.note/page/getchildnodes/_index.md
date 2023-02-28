---
title: Page.GetChildNodes
second_title: Aspose.Note for .NET API Referansı
description: Page yöntem. Sayfanın tüm alt düğümlerini düğüm türüne göre alın.
type: docs
weight: 150
url: /tr/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Sayfanın tüm alt düğümlerini düğüm türüne göre alın.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parametre | Tanım |
| --- | --- |
| T1 | Döndürülen listedeki öğelerin türü. |

### Geri dönüş değeri

Alt düğümlerin listesi.

### Örnekler

Tüm metnin belgeden nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Metni al
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Çıktı ekranındaki metni yazdır
Console.WriteLine(text);
```

Sayfadaki tüm metnin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Sayfa düğümlerinin listesini al
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Metni al
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Çıktı ekranındaki metni yazdır
    Console.WriteLine(text);
}
```

Tüm sayfaların nasıl geçileceğini ve metinde nasıl değiştirileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm RichText düğümlerini al
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Bir şeklin metnini değiştir
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Desteklenen herhangi bir dosya biçiminde kaydedin
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Sayfa metninin nasıl geçileceğini ve değiştirileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Tüm RichText düğümlerini al
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Bir şeklin metnini değiştir
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Desteklenen herhangi bir dosya biçiminde kaydedin
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Ayrıca bakınız

* interface [INode](../../inode/)
* class [Page](../)
* ad alanı [Aspose.Note](../../page/)
* toplantı [Aspose.Note](../../../)


