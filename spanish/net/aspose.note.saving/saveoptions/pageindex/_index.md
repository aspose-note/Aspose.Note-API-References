---
title: PageIndex
second_title: Aspose.Note para la referencia de la API de .NET
description: Obtiene o establece el índice de la primera página a guardar. Por defecto es 0.
type: docs
weight: 30
url: /es/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Obtiene o establece el índice de la primera página a guardar. Por defecto es 0.

```csharp
public int PageIndex { get; set; }
```

### Ejemplos

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

Muestra cómo crear un documento con texto enriquecido formateado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Page page = new Page();

// Inicializa el objeto de la clase Título
Title title = new Title();

// Inicializa el objeto de la clase TextStyle y establece las propiedades de formato
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// Establecer el título de la página
page.Title = title;

// Agregar nodo de texto enriquecido
outlineElem.AppendChildLast(text);

// Agregar nodo de elemento de esquema
outline.AppendChildLast(outlineElem);

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Ver también

* class [SaveOptions](../../saveoptions)
* espacio de nombres [Aspose.Note.Saving](../../saveoptions)
* asamblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
