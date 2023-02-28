---
title: Document.Print
second_title: Aspose.Note para la referencia de la API de .NET
description: Document método. Imprime el documento utilizando la impresora predeterminada.
type: docs
weight: 130
url: /es/net/aspose.note/document/print/
---
## Print() {#print}

Imprime el documento utilizando la impresora predeterminada.

```csharp
public void Print()
```

### Ejemplos

Muestra cómo enviar un documento a una impresora utilizando el cuadro de diálogo estándar de Windows con opciones predeterminadas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Imprime el documento utilizando la impresora predeterminada.

```csharp
public void Print(PrintOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| options | PrintOptions | Opciones utilizadas para imprimir un documento. Puede ser nulo. |

### Ver también

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


