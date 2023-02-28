---
title: MergeOptions.InsertAt
second_title: Aspose.Note für .NET-API-Referenz
description: MergeOptions eigendom. Ermittelt oder legt die Position fest an der importierte Seiten eingefügt werden.
type: docs
weight: 40
url: /de/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

Ermittelt oder legt die Position fest, an der importierte Seiten eingefügt werden.

```csharp
public int InsertAt { get; set; }
```

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException |  |

### Bemerkungen

Wenn der Wert größer als die Anzahl der Seiten im Zieldokument ist, werden importierte Seiten am Ende des Dokuments hinzugefügt.

### Beispiele

Zeigt, wie alle Seiten aus einer Reihe von PDF-Dokumenten importiert werden, während Seiten aus jedem PDF-Dokument als untergeordnete Elemente einer OneNote-Seite der obersten Ebene eingefügt werden.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

### Siehe auch

* class [MergeOptions](../)
* namensraum [Aspose.Note](../../mergeoptions/)
* Montage [Aspose.Note](../../../)


