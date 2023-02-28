---
title: Class MergeOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.MergeOptions klas. Die Optionen zum Zusammenführen einer Sammlung von Seiten.
type: docs
weight: 340
url: /de/net/aspose.note/mergeoptions/
---
## MergeOptions class

Die Optionen zum Zusammenführen einer Sammlung von Seiten.

```csharp
public class MergeOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob bereitgestellte Seiten als einzelne Seite importiert werden sollen. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob eingefügte Seiten als untergeordnete Seiten der vorherigen Seite hinzugefügt werden sollen. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Ermittelt oder legt die Position fest, an der importierte Seiten eingefügt werden. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Ruft den Abstand zwischen Seiten ab oder legt ihn fest, wenn er als einzelne Seite importiert wird. |

### Beispiele

Zeigt, wie alle Seiten aus einem PDF-Dokument importiert werden, das alle 5 Seiten auf eine einzelne OneNote-Seite gruppiert.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

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

Zeigt, wie der gesamte Inhalt aus einer Reihe von PDF-Dokumenten importiert wird, während Seiten aus allen PDF-Dokumenten zu einer einzigen OneNote-Seite zusammengeführt werden.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### Siehe auch

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


