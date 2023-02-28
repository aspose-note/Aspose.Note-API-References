---
title: MergeOptions.InsertAsChild
second_title: Référence de l'API Aspose.Note pour .NET
description: MergeOptions propriété. Obtient ou définit une valeur indiquant si les pages insérées doivent être ajoutées en tant quenfants de la page précédente.
type: docs
weight: 30
url: /fr/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Obtient ou définit une valeur indiquant si les pages insérées doivent être ajoutées en tant qu'enfants de la page précédente.

```csharp
public bool InsertAsChild { get; set; }
```

### Exemples

Montre comment importer toutes les pages d'un ensemble de documents PDF tout en insérant des pages de chaque document PDF en tant qu'enfants d'une page OneNote de niveau supérieur.

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

### Voir également

* class [MergeOptions](../)
* espace de noms [Aspose.Note](../../mergeoptions/)
* Assemblée [Aspose.Note](../../../)


