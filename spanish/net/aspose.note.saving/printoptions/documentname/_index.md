---
title: PrintOptions.DocumentName
second_title: Aspose.Note para la referencia de la API de .NET
description: PrintOptions propiedad. Obtiene o establece el nombre del documento que se mostrará por ejemplo en un cuadro de diálogo de estado de impresión o en la cola de la impresora mientras se imprime el documento.
type: docs
weight: 20
url: /es/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Obtiene o establece el nombre del documento que se mostrará (por ejemplo, en un cuadro de diálogo de estado de impresión o en la cola de la impresora) mientras se imprime el documento.

```csharp
public string DocumentName { get; set; }
```

### Ejemplos

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

### Ver también

* class [PrintOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../printoptions/)
* asamblea [Aspose.Note](../../../)


