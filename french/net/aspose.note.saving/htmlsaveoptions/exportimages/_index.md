---
title: HtmlSaveOptions.ExportImages
second_title: Référence de l'API Aspose.Note pour .NET
description: HtmlSaveOptions propriété. Obtient ou définit la façon dont les images sont exportées.
type: docs
weight: 70
url: /fr/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Obtient ou définit la façon dont les images sont exportées.

```csharp
public ResourceExportType ExportImages { get; set; }
```

### Exemples

Montre comment enregistrer un document au format html en stockant toutes les ressources (css/fonts/images) dans des fichiers séparés.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Montre comment enregistrer un document dans un flux au format html avec intégration de toutes les ressources (css/fonts/images).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

### Voir également

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* espace de noms [Aspose.Note.Saving](../../htmlsaveoptions/)
* Assemblée [Aspose.Note](../../../)


