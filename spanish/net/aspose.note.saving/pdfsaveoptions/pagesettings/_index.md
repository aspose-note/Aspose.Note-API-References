---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note para la referencia de la API de .NET
description: PdfSaveOptions propiedad. Obtiene o establece la configuración de página para cada página en el documento. De manera predeterminada depende de CurrentUICulture las culturas de EE. UU. tienen una configuración de letra otras tienen una configuración de A4.
type: docs
weight: 40
url: /es/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Obtiene o establece la configuración de página para cada página en el documento. De manera predeterminada, depende de CurrentUICulture, *las culturas de EE. UU. tienen una configuración de letra, otras tienen una configuración de A4.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../pdfsaveoptions/)
* asamblea [Aspose.Note](../../../)


