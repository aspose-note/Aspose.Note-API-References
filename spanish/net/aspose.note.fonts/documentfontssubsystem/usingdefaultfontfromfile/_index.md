---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note para la referencia de la API de .NET
description: DocumentFontsSubsystem método. Crear una nueva instancia de DocumentFontsSubsystem usando una fuente del archivo especificado como predeterminado.
type: docs
weight: 40
url: /es/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Crear una nueva instancia de DocumentFontsSubsystem usando una fuente del archivo especificado como predeterminado.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | El archivo que contiene el nombre de fuente predeterminado. |
| fontsSubstitutions | Dictionary`2 | Las sustituciones de fuentes. |

### Valor_devuelto

El[`DocumentFontsSubsystem`](../) .

### Ejemplos

Muestra cómo guardar un documento en formato pdf utilizando la fuente predeterminada de un archivo.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Guarda el documento como PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### Ver también

* class [DocumentFontsSubsystem](../)
* espacio de nombres [Aspose.Note.Fonts](../../documentfontssubsystem/)
* asamblea [Aspose.Note](../../../)


