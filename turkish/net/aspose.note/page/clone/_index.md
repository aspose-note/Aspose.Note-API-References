---
title: Page.Clone
second_title: Aspose.Note for .NET API Referansı
description: Page yöntem. Sayfayı klonlar.
type: docs
weight: 140
url: /tr/net/aspose.note/page/clone/
---
## Page.Clone method

Sayfayı klonlar.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| cloneHistory | Boolean | Sayfa geçmişinin kopyalanıp kopyalanmayacağını belirtir.. |

### Geri dönüş değeri

Sayfanın bir kopyası.

### Örnekler

Bir sayfanın geçerli sürümünün geçmişe nasıl gönderileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin ve ilk çocuğu alın           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Bir sayfanın nasıl kopyalanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Geçmiş olmadan yeni belgeye kopyala
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Geçmişi olan yeni belgeye kopyala
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Ayrıca bakınız

* class [Page](../)
* ad alanı [Aspose.Note](../../page/)
* toplantı [Aspose.Note](../../../)


