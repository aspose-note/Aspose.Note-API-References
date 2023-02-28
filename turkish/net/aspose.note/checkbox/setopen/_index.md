---
title: CheckBox.SetOpen
second_title: Aspose.Note for .NET API Referansı
description: CheckBox yöntem. Etiketi durumu açacak şekilde ayarlar.
type: docs
weight: 80
url: /tr/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Etiketi durumu açacak şekilde ayarlar.

```csharp
public virtual void SetOpen()
```

### Örnekler

'C Projesi' ile ilgili tüm onay kutusu öğelerinin nasıl açılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

### Ayrıca bakınız

* class [CheckBox](../)
* ad alanı [Aspose.Note](../../checkbox/)
* toplantı [Aspose.Note](../../../)


