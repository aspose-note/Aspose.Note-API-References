---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note para la referencia de la API de .NET
description: PageSettings propiedad. Obtiene la configuración para la página de formato A4 con altura ilimitada.
type: docs
weight: 20
url: /es/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Obtiene la configuración para la página de formato A4 con altura ilimitada.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Ejemplos

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

* class [PageSettings](../)
* espacio de nombres [Aspose.Note.Saving](../../pagesettings/)
* asamblea [Aspose.Note](../../../)


