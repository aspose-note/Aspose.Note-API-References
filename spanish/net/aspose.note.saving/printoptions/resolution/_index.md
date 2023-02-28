---
title: PrintOptions.Resolution
second_title: Aspose.Note para la referencia de la API de .NET
description: PrintOptions propiedad. Obtiene o establece la resolución de las imágenes generadas en puntos por pulgada.
type: docs
weight: 50
url: /es/net/aspose.note.saving/printoptions/resolution/
---
## PrintOptions.Resolution property

Obtiene o establece la resolución de las imágenes generadas, en puntos por pulgada.

```csharp
public float Resolution { get; set; }
```

### Observaciones

El valor predeterminado es 96.

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


