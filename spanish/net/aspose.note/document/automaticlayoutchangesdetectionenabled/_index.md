---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note para la referencia de la API de .NET
description: Document propiedad. Obtiene o establece un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente. El valor predeterminado esverdadero .
type: docs
weight: 20
url: /es/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Obtiene o establece un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente. El valor predeterminado es`verdadero` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### Ejemplos

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

// Guarde el documento de OneNote en diferentes formatos, establezca el tamaño de fuente del texto y detecte los cambios de diseño manualmente.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


