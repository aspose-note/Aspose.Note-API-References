---
title: RichText.LastModifiedTime
second_title: Aspose.Note for .NET API Referansı
description: RichText mülk. Son değiştirilme zamanını alır veya ayarlar.
type: docs
weight: 30
url: /tr/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Son değiştirilme zamanını alır veya ayarlar.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Örnekler

En son metin değişikliklerini vurgulayarak vurgulayalım.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Aspose.one");

// RichText düğümlerinin geçen hafta değiştirilmesini sağlayın.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Vurgu rengini ayarla
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Vurgu rengini ayarla
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Ayrıca bakınız

* class [RichText](../)
* ad alanı [Aspose.Note](../../richtext/)
* toplantı [Aspose.Note](../../../)


