---
title: PrintOptions.PageSplittingAlgorithm
second_title: Aspose.Note para la referencia de la API de .NET
description: PrintOptions propiedad. Obtiene o establece el algoritmo utilizado para la división de páginas.
type: docs
weight: 30
url: /es/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

Obtiene o establece el algoritmo utilizado para la división de páginas.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### El valor de la propiedad

El`PageSplittingAlgorithm` .

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

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../printoptions/)
* asamblea [Aspose.Note](../../../)


