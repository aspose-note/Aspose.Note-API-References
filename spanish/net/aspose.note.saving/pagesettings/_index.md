---
title: Class PageSettings
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Saving.PageSettings clase. Representa la configuración de diseño de una página.
type: docs
weight: 820
url: /es/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Representa la configuración de diseño de una página.

```csharp
public class PageSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Obtiene la configuración para la página en formato A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Obtiene la configuración para la página de formato A4 con altura ilimitada. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Obtiene la configuración para la página en formato Carta. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Obtiene la configuración para la página de formato Carta con altura ilimitada. |

### Ejemplos

Muestra cómo guardar un documento en formato PDF con diseño de página Carta.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Guarda el documento.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Muestra cómo guardar un documento en formato PDF con diseño de página A4 sin límite de altura.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Guarda el documento.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Ver también

* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving/)
* asamblea [Aspose.Note](../../)


