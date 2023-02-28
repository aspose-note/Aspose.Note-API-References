---
title: Page.Author
second_title: Aspose.Note for .NET API Referansı
description: Page mülk. Yazarı alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note/page/author/
---
## Page.Author property

Yazarı alır veya ayarlar.

```csharp
public string Author { get; set; }
```

### Örnekler

Bir sayfa hakkında meta bilgilerin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Sayfa geçmişinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// İlk sayfayı al
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Ayrıca bakınız

* class [Page](../)
* ad alanı [Aspose.Note](../../page/)
* toplantı [Aspose.Note](../../../)


