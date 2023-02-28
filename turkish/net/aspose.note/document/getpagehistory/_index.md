---
title: Document.GetPageHistory
second_title: Aspose.Note for .NET API Referansı
description: Document yöntem. Şunu alırPageHistory bir belgede sunulan her sayfa için tam geçmişi içeren en erken dizin 0. Geçerli sayfa revizyonuna şu şekilde erişilebilirCurrent ve geçmiş sürümlerin koleksiyonundan ayrı olarak yer alır.
type: docs
weight: 100
url: /tr/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Şunu alır:[`PageHistory`](../../pagehistory/) bir belgede sunulan her sayfa için tam geçmişi içeren (en erken dizin 0). Geçerli sayfa revizyonuna şu şekilde erişilebilir:[`Current`](../../pagehistory/current/) ve geçmiş sürümlerin koleksiyonundan ayrı olarak yer alır.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| page | Page | Bir sayfanın mevcut revizyonu. |

### Geri dönüş değeri

[`PageHistory`](../../pagehistory/) .

### Örnekler

Bir sayfanın önceki sürümünün nasıl geri yükleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin ve ilk çocuğu alın           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Sayfa geçmişinin nasıl düzenleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin ve ilk çocuğu alın           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Bir sayfanın çakışma sayfası olup olmadığının nasıl kontrol edileceğini gösterir (yani, OneNote'un otomatik olarak birleştiremediği değişiklikler içerir).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Varsayılan olarak çakışma sayfaları kaydedilirken atlanır.
    // Çakışmasız olarak işaretlerseniz, geçmişe her zamanki gibi kaydedilecektir.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Ayrıca bakınız

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


