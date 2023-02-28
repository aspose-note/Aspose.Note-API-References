---
title: MergeOptions.PageSpacing
second_title: Aspose.Note für .NET-API-Referenz
description: MergeOptions eigendom. Ruft den Abstand zwischen Seiten ab oder legt ihn fest wenn er als einzelne Seite importiert wird.
type: docs
weight: 50
url: /de/net/aspose.note/mergeoptions/pagespacing/
---
## MergeOptions.PageSpacing property

Ruft den Abstand zwischen Seiten ab oder legt ihn fest, wenn er als einzelne Seite importiert wird.

```csharp
public float PageSpacing { get; set; }
```

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

* class [MergeOptions](../)
* namensraum [Aspose.Note](../../mergeoptions/)
* Montage [Aspose.Note](../../../)


