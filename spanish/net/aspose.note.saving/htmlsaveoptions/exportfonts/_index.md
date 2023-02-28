---
title: HtmlSaveOptions.ExportFonts
second_title: Aspose.Note para la referencia de la API de .NET
description: HtmlSaveOptions propiedad. Obtiene o establece la forma en que se exportan las fuentes.
type: docs
weight: 60
url: /es/net/aspose.note.saving/htmlsaveoptions/exportfonts/
---
## HtmlSaveOptions.ExportFonts property

Obtiene o establece la forma en que se exportan las fuentes.

```csharp
public ResourceExportType ExportFonts { get; set; }
```

### Ejemplos

Muestra cómo guardar un documento en formato html con el almacenamiento de todos los recursos (css/fuentes/imágenes) en archivos separados.

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

Muestra cómo guardar un documento en una secuencia en formato html con la incorporación de todos los recursos (css/fonts/images).

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

### Ver también

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../htmlsaveoptions/)
* asamblea [Aspose.Note](../../../)


