---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Fonts.DocumentFontsSubsystem clase. Implementación simple de Aspose.Note.Fonts.FontsSubsystem. recuperaFontFamily objeto de OS.
type: docs
weight: 100
url: /es/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Implementación simple de Aspose.Note.Fonts.FontsSubsystem. recuperaFontFamily objeto de OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Inicializa una nueva instancia del`DocumentFontsSubsystem` clase. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Inicializa una nueva instancia del`DocumentFontsSubsystem` clase. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Inicializa una nueva instancia del`DocumentFontsSubsystem` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Obtiene o establece la instancia predeterminada estática. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Obtiene o establece la fuente predeterminada. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Crear una nueva instancia de DocumentFontsSubsystem utilizando el nombre de fuente predeterminado especificado. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Crear una nueva instancia de DocumentFontsSubsystem usando una fuente del archivo especificado como predeterminado. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Crear una nueva instancia de DocumentFontsSubsystem utilizando una fuente del flujo especificado como predeterminado. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Agrega la fuente. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Agrega la fuente. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Agrega la fuente. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Agrega sustitución de fuente. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Obtiene la familia de fuentes. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Carga todas las fuentes TrueType de la carpeta especificada a la colección interna. |

### Ejemplos

Muestra cómo guardar un documento en formato pdf utilizando la fuente predeterminada especificada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Guarda el documento como PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

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

* class [FontsSubsystem](../fontssubsystem/)
* espacio de nombres [Aspose.Note.Fonts](../../aspose.note.fonts/)
* asamblea [Aspose.Note](../../)


