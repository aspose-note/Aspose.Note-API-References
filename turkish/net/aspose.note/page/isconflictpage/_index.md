---
title: Page.IsConflictPage
second_title: Aspose.Note for .NET API Referansı
description: Page mülk. Bu sayfanın bir çakışma sayfası olup olmadığını gösteren bir değer alır veya ayarlar.
type: docs
weight: 50
url: /tr/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Bu sayfanın bir çakışma sayfası olup olmadığını gösteren bir değer alır veya ayarlar.

```csharp
public bool IsConflictPage { get; set; }
```

### Notlar

Çakışma sayfası, iki kullanıcı aynı içeriği güncellemeye çalıştığında ortaya çıkar. Bu durumda ilk kullanıcının değişiklikleri her zamanki gibi yazılır. Ancak başka bir kullanıcının değişiklikleri birleştirilemez. Böylece sayfanın yalnızca bir kopyası oluşturulur ve çakışma olarak işaretlendi.

Bu sürümde, çakışmalar ilk kullanıcının değişiklikleri lehine çözülür. Dolayısıyla, belgede çakışan sayfalar varsa, bunlar geçmişte gösterilecek ancak kaydetme sırasında atlanacaktır. Bu sayfaları kaydetmek için bu bayrağı sıfırlamak mümkündür. tarihte her zamanki gibi.

Çakışmaya göre manipüle etmenin ayrıntılı örneği sayfası çevrimiçi belgelerde bulunabilir.

### Örnekler

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

* class [Page](../)
* ad alanı [Aspose.Note](../../page/)
* toplantı [Aspose.Note](../../../)


