---
title: CheckBox.SetCompleted
second_title: Aspose.Note for .NET API Referansı
description: CheckBox yöntem. Etiketi tamamlanmış duruma ayarlar.
type: docs
weight: 70
url: /tr/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Etiketi tamamlanmış duruma ayarlar.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| completedTime | DateTime | Tamamlanan süre. |

### Ayrıca bakınız

* class [CheckBox](../)
* ad alanı [Aspose.Note](../../checkbox/)
* toplantı [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Geçerli saati tamamlanma süresi olarak kullanarak etiketi tamamlanmış duruma ayarlar.

```csharp
public void SetCompleted()
```

### Örnekler

'C Projesi' ile ilgili tüm onay kutusu öğelerinin nasıl tamamlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

### Ayrıca bakınız

* class [CheckBox](../)
* ad alanı [Aspose.Note](../../checkbox/)
* toplantı [Aspose.Note](../../../)


