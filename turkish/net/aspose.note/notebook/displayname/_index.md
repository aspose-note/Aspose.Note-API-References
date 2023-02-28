---
title: Notebook.DisplayName
second_title: Aspose.Note for .NET API Referansı
description: Notebook mülk. Görünen adı alır veya ayarlar.
type: docs
weight: 40
url: /tr/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Görünen adı alır veya ayarlar.

```csharp
public string DisplayName { get; set; }
```

### Örnekler

Not defterinden bir bölümün nasıl kaldırılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "test.onetoc2");

// İstenen alt öğeyi aramak için alt düğümleri arasında gezinin
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Alt Öğeyi Defterden Kaldır
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Not Defterini Kaydet
notebook.Save(dataDir);
```

### Ayrıca bakınız

* class [Notebook](../)
* ad alanı [Aspose.Note](../../notebook/)
* toplantı [Aspose.Note](../../../)


