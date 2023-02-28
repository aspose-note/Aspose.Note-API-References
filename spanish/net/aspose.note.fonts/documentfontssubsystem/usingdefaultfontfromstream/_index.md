---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note para la referencia de la API de .NET
description: DocumentFontsSubsystem método. Crear una nueva instancia de DocumentFontsSubsystem utilizando una fuente del flujo especificado como predeterminado.
type: docs
weight: 50
url: /es/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Crear una nueva instancia de DocumentFontsSubsystem utilizando una fuente del flujo especificado como predeterminado.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| defaultFontStream | Stream | El flujo que contiene el nombre de fuente predeterminado. |
| fontsSubstitutions | Dictionary`2 | Las sustituciones de fuentes. |

### Valor_devuelto

El[`DocumentFontsSubsystem`](../) .

### Ejemplos

Muestra cómo guardar un documento en formato pdf utilizando la fuente predeterminada de una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Guarda el documento como PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Ver también

* class [DocumentFontsSubsystem](../)
* espacio de nombres [Aspose.Note.Fonts](../../documentfontssubsystem/)
* asamblea [Aspose.Note](../../../)


