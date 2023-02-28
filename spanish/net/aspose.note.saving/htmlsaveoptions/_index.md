---
title: Class HtmlSaveOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Saving.HtmlSaveOptions clase. Permite especificar opciones adicionales al guardar el documento en formato HTML.
type: docs
weight: 700
url: /es/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Permite especificar opciones adicionales al guardar el documento en formato HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Obtiene o establece si el archivo StyleSheet se generará para cada nueva página por separado. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Obtiene o establece un valor que indica si la generación de documentos por página está habilitada. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Obtiene o establece la forma en que se exporta css. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Obtiene o establece la forma en que se exportan las fuentes. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Obtiene o establece la forma en que se exportan las imágenes. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Obtiene o establece los tipos de letra de la fuente. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar la fuente. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Obtiene o establece la configuración de la fuente que se usará al guardar |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar la imagen. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar. Por defecto esMaxValue lo que significa que se procesarán todas las páginas del documento. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Obtiene o establece el índice de la primera página a guardar. Por defecto es 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar la página. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Obtiene el formato en el que se guarda el documento. |

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

Muestra cómo crear un documento y guardarlo en un rango de páginas especificado en formato html.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inicializa el documento de OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Estilo predeterminado para todo el texto del documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Guardar en formato HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Muestra cómo guardar un documento en formato html con el almacenamiento de todos los recursos (css/fuentes/imágenes) mediante el uso de devoluciones de llamada definidas por el usuario.

```csharp
// El siguiente código crea la carpeta 'documentFolder' que contiene document.html, la carpeta 'css' con el archivo 'style.css', la carpeta 'images' con imágenes y la carpeta 'fonts' con fuentes.
// El archivo 'style.css' contendrá al final la siguiente cadena "/* Esta línea se agrega a la transmisión manualmente por el usuario */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving/)
* asamblea [Aspose.Note](../../)


