---
title: RevisionSummary
second_title: Aspose.Note for .NET API Referansı
description: Düğümün revizyonu için bir özeti temsil eder.
type: docs
weight: 500
url: /tr/net/aspose.note/revisionsummary/
---
## RevisionSummary class

Düğümün revizyonu için bir özeti temsil eder.

```csharp
public class RevisionSummary
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [RevisionSummary](revisionsummary)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent) { get; set; } | En son yazarı alır veya ayarlar. |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |

### Örnekler

Sayfanın meta bilgilerinin nasıl düzenleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle ve ilk çocuğu al           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Bu sayfa için İçerik Revizyon Özeti Okuma
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

Bir sayfanın çakışma sayfası olup olmadığının nasıl kontrol edileceğini gösterir (yani, OneNote'un otomatik olarak birleştiremeyeceği değişikliklere sahiptir).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle
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

    // Varsayılan olarak çakışan sayfalar kaydedilirken atlanır.
    // Çakışmaz olarak işaretlerseniz, tarihte her zamanki gibi kaydedilecektir.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Ayrıca bakınız

* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->