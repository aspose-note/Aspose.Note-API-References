---
title: Document
second_title: Aspose.Note para la referencia de la API de .NET
description: Representa un documento Aspose.Note.
type: docs
weight: 60
url: /es/net/aspose.note/document/
---
## Document class

Representa un documento Aspose.Note.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Document](document#constructor)() | Inicializa una nueva instancia del[`Document`](../document) class. Crea un documento de OneNote en blanco. |
| [Document](document#constructor_1)(Stream) | Inicializa una nueva instancia del[`Document`](../document) class. Abre un documento de OneNote existente desde una secuencia. |
| [Document](document#constructor_3)(string) | Inicializa una nueva instancia del[`Document`](../document) class. Abre un documento de OneNote existente desde un archivo. |
| [Document](document#constructor_2)(Stream, LoadOptions) | Inicializa una nueva instancia del[`Document`](../document) class. Abre un documento de OneNote existente desde una secuencia. Permite especificar opciones adicionales como una contraseña de cifrado. |
| [Document](document#constructor_4)(string, LoadOptions) | Inicializa una nueva instancia del[`Document`](../document) class. Abre un documento de OneNote existente desde un archivo. Permite especificar opciones adicionales como una contraseña de cifrado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | Obtiene o establece un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente. El valor predeterminado es`verdadero` . |
| [Color](../../aspose.note/document/color) { get; set; } | Obtiene o establece el color. |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | Obtiene o establece la hora de creación. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | Obtiene o establece el nombre para mostrar. |
| [Document](../../aspose.note/node/document) { get; } | Obtiene el documento del nodo. |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | Obtiene el formato de archivo (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | Obtiene la identificación única global del objeto. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Obtiene el siguiente nodo en el mismo nivel de árbol de nodos. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Obtiene el tipo de nodo. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Obtiene el nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Obtiene el nodo anterior en el mismo nivel de árbol de nodos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | Acepta al visitante del nodo. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | Detecta todos los cambios realizados en el diseño del documento desde la anterior[`DetectLayoutChanges`](./detectlayoutchanges) call. Por si acaso[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) establecido en verdadero, utilizado automáticamente al comienzo de la exportación del documento. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | Obtiene el[`PageHistory`](../pagehistory) que contiene el historial completo de cada página presentada en un documento (la más antigua en el índice 0). Se puede acceder a la revisión de la página actual como[`Current`](../pagehistory/current) contenido por separado de la colección de versiones históricas. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | Importa un conjunto de páginas del documento PDF proporcionado. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | Importa un conjunto de páginas del documento PDF proporcionado. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | Fusiona un conjunto de páginas con el documento. |
| [Print](../../aspose.note/document/print#print)() | Imprime el documento utilizando la impresora predeterminada. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | Imprime el documento utilizando la impresora predeterminada. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | Guarda el documento de OneNote en una secuencia. |
| [Save](../../aspose.note/document/save#save_3)(string) | Guarda el documento de OneNote en un archivo. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | Guarda el documento de OneNote en una secuencia en el formato especificado. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | Guarda el documento de OneNote en una secuencia con las opciones de guardado especificadas. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | Guarda el documento de OneNote en un archivo con el formato especificado. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | Guarda el documento de OneNote en un archivo usando las opciones de guardado especificadas. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | Comprueba si un documento de un flujo está encriptado. Para verificarlo, necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | Comprueba si un documento de un archivo está encriptado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | Comprueba si un documento de un flujo está encriptado. Para verificarlo, necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | Comprueba si un documento de un flujo está encriptado. Para verificarlo, necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | Comprueba si un documento de un archivo está encriptado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | Comprueba si un documento de un archivo está encriptado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento. |

### Ejemplos

Muestra cómo enviar un documento a una impresora utilizando el cuadro de diálogo estándar de Windows con opciones predeterminadas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Muestra cómo guardar un documento.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Muestra cómo un documento encriptado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Muestra cómo guardar un documento con cifrado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Muestra cómo guardar un documento mediante la enumeración SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Muestra cómo guardar un documento usando OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Muestra cómo obtener el recuento de páginas de un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener el numero de paginas
int count = oneFile.Count();

// Imprime el conteo en la pantalla de salida
Console.WriteLine(count);
```

Muestra cómo guardar un documento en formato pdf utilizando la configuración predeterminada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Guarda el documento como PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Muestra cómo guardar un documento en formato gif.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Guarda el documento como gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Muestra cómo establecer una calidad de imagen al guardar un documento como imagen en formato JPEG.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Guarda el documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Muestra cómo establecer una resolución de imagen al guardar un documento como imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Guarda el documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Muestra cómo obtener el formato de archivo de un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Procesar OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Procesar OneNote en línea
        break;
}
```

Muestra cómo vincular un hipervínculo a una imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://imagen.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Muestra cómo guardar un documento en una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Rebobinar la posición de la transmisión a cero para que esté lista para el próximo lector.
dstStream.Seek(0, SeekOrigin.Begin);
```

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo agregar una nueva sección a un cuaderno.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Agregar un nuevo hijo al Cuaderno
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Guardar el cuaderno
notebook.Save(dataDir);
```

Muestra cómo verificar si la carga de un documento falla porque el formato de OneNote 2007 no es compatible.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

Muestra cómo restaurar la versión anterior de una página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Muestra cómo clonar una página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargar documento de OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Clonar en un nuevo documento sin historial
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Clonar en un nuevo documento con historial
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

Muestra cómo configurar la descripción del texto para una imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Muestra cómo obtener metainformación sobre una página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Cuando las páginas largas de OneNote se guardan en formato pdf, se dividen en páginas. El ejemplo muestra cómo configurar la lógica de división de objetos ubicados en los saltos de página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// o
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Muestra cómo guardar un documento en formato png.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inicializa el objeto ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Establecer el índice de la página
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Guarda el documento como PNG.
oneFile.Save(dataDir, opts);
```

Muestra cómo editar el historial de la página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

Muestra cómo pasar el contenido de un bloc de notas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Hacer algo con el documento secundario
        }
        else if (notebookChildNode is Notebook)
        {
            // Hacer algo con el cuaderno del niño
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

Muestra cómo obtener una imagen de un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener todos los nodos de imagen
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Guardar bytes de imagen en un archivo
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Muestra cómo guardar un documento en formato pdf.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inicializa el objeto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Establecer el índice de página de la primera página que se guardará
                              PageIndex = 0,

                              // Establecer el número de páginas
                              PageCount = 1,
                          };

// Guarda el documento como PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Muestra cómo guardar un documento en formato pdf usando configuraciones específicas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inicializa el objeto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Usar compresión JPEG
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Calidad para compresión JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Muestra cómo enviar un documento a una impresora mediante el cuadro de diálogo estándar de Windows con opciones específicas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

Muestra cómo obtener la metainformación de la imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener todos los nodos de imagen
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Muestra cómo obtener el contenido de un archivo adjunto.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Attachments();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Obtener una lista de nodos de archivos adjuntos
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterar a través de todos los nodos
foreach (AttachedFile file in nodes)
{
    // Cargar archivo adjunto a un objeto de flujo
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Crear un archivo local
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copiar secuencia de archivos
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Muestra cómo obtener el historial de la página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargar documento de OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Obtener la primera página
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

Muestra cómo agregar un archivo a un documento mediante la ruta de archivo.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inicializa el objeto de la clase AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Agregar archivo adjunto
outlineElem.AppendChildLast(attachedFile);

// Agregar nodo de elemento de esquema
outline.AppendChildLast(outlineElem);

// Agregar nodo de esquema
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Muestra cómo crear un documento y guardarlo en formato html usando las opciones predeterminadas.

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Muestra cómo verificar si una página es una página en conflicto (es decir, tiene cambios que OneNote no pudo fusionar automáticamente).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Cargar documento de OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Por defecto, las páginas de conflicto simplemente se omiten al guardar.
    // Si lo marca como sin conflicto, se guardará como de costumbre en el historial.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Muestra cómo agregar una imagen desde un archivo a un documento con propiedades definidas por el usuario.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Cargar documento desde la secuencia.
Document doc = new Document(dataDir + "Aspose.one");

// Obtener la primera página del documento.
Aspose.Note.Page page = doc.FirstChild;

// Carga una imagen del archivo.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Cambia el tamaño de la imagen según tus necesidades (opcional).
                              Width = 100,
                              Height = 100,

                              // Establecer la ubicación de la imagen en la página (opcional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Establecer la alineación de la imagen
                              Alignment = HorizontalAlignment.Right
                          };

// Agrega la imagen a la página.
page.AppendChildLast(image);
```

Muestra cómo agregar un archivo de una secuencia a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Inicializa el objeto de clase AttachedFile y también pasa su ruta de icono
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Agregar archivo adjunto
    outlineElem.AppendChildLast(attachedFile);
}

// Agregar nodo de elemento de esquema
outline.AppendChildLast(outlineElem);

// Agregar nodo de esquema
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Cuando las páginas largas de OneNote se guardan en formato pdf, se dividen en páginas. El ejemplo muestra cómo configurar la lógica de división de objetos ubicados en los saltos de página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
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

Muestra cómo crear un documento con página titulada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crear un objeto de la clase Documento
Document doc = new Aspose.Note.Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Estilo predeterminado para todo el texto del documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Establecer las propiedades del título de la página
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Agregar nodo de página en el documento
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Muestra cómo agregar una imagen de una secuencia a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Cargue la segunda imagen usando el nombre de la imagen, la extensión y la transmisión.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Establecer la alineación de la imagen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Muestra cómo agregar una imagen de un archivo a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema y establece las propiedades de compensación
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carga una imagen por la ruta del archivo.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Establecer la alineación de la imagen
                              Alignment = HorizontalAlignment.Right
                          };

// Añadir imagen
outlineElem.AppendChildLast(image);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem);

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Muestra cómo crear un documento con un texto.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Page page = new Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inicializa el objeto de la clase TextStyle y establece las propiedades de formato
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inicializa el objeto de la clase RichText y aplica el estilo de texto
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Agregar nodo de texto enriquecido
outlineElem.AppendChildLast(text);

// Agregar nodo de elemento de esquema
outline.AppendChildLast(outlineElem);

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Muestra cómo guardar un documento en diferentes formatos.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inicializar el nuevo documento
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Inicializar la nueva página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Estilo predeterminado para todo el texto del documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Agregar nodo de página
doc.AppendChildLast(page);

// Guarde el documento de OneNote en diferentes formatos, configure el tamaño de fuente del texto y detecte los cambios de diseño manualmente.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

Muestra cómo vincular un hipervínculo a un texto.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crear un objeto de la clase Documento
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem);

// Inicializa el objeto de la clase Título
Title title = new Title() { TitleText = titleText };

// Inicializar objeto de clase de página
Page page = new Note.Page() { Title = title };

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Muestra cómo acceder al contenido de un documento utilizando el visitante.

```csharp
public static void Run()
{
    // La ruta al directorio de documentos.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Abre el documento que queremos convertir.
    Document doc = new Document(dataDir + "Aspose.one");

    // Crear un objeto que herede de la clase DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Este es el conocido patrón Visitante. Obtenga el modelo para aceptar un visitante.
    // El modelo iterará a través de sí mismo llamando a los métodos correspondientes
    // en el objeto visitante (esto se llama visita).
    //
    // Tenga en cuenta que cada nodo en el modelo de objetos tiene el método Aceptar, por lo que la visita
    // puede ejecutarse no solo para todo el documento, sino también para cualquier nodo del documento.
    doc.Accept(myConverter);

    // Una vez completada la visita, podemos recuperar el resultado de la operación,
    // que en este ejemplo, se ha acumulado en el visitante.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Implementación simple de guardar un documento en formato de texto sin formato. Implementado como Visitante.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// Obtiene el texto sin formato del documento que fue acumulado por el visitante.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Agrega texto a la salida actual. Respeta el indicador de salida activado/desactivado.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo RichText en el documento.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo Documento en el documento.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo de página en el documento.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Llamado cuando finaliza el procesamiento de un nodo de página.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo Título en el documento.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo de imagen en el documento.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo de OutlineGroup en el documento.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo Esquema en el documento.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo OutlineElement en el documento.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Obtiene el conteo total de nodos por parte del Visitante
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### Ver también

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* espacio de nombres [Aspose.Note](../../aspose.note)
* asamblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
