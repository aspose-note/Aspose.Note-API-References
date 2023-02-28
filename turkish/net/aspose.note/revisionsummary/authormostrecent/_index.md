---
title: RevisionSummary.AuthorMostRecent
second_title: Aspose.Note for .NET API Referansı
description: RevisionSummary mülk. En son yazarı alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note/revisionsummary/authormostrecent/
---
## RevisionSummary.AuthorMostRecent property

En son yazarı alır veya ayarlar.

```csharp
public string AuthorMostRecent { get; set; }
```

### Örnekler

Sayfanın meta bilgilerinin nasıl düzenleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin ve ilk çocuğu alın           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Bu sayfa için İçerik Revizyon Özeti okunuyor
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Bu sayfa için Sayfa Revizyon Özetini güncelle
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

* class [RevisionSummary](../)
* ad alanı [Aspose.Note](../../revisionsummary/)
* toplantı [Aspose.Note](../../../)


