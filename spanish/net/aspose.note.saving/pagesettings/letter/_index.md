---
title: PageSettings.Letter
second_title: Aspose.Note para la referencia de la API de .NET
description: PageSettings propiedad. Obtiene la configuración para la página en formato Carta.
type: docs
weight: 30
url: /es/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Obtiene la configuración para la página en formato Carta.

```csharp
public static PageSettings Letter { get; }
```

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

### Ver también

* class [PageSettings](../)
* espacio de nombres [Aspose.Note.Saving](../../pagesettings/)
* asamblea [Aspose.Note](../../../)


