---
title: Enum FileFormat
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.FileFormat enumeración. Representa el formato de archivo de OneNote.
type: docs
weight: 90
url: /es/net/aspose.note/fileformat/
---
## FileFormat enumeration

Representa el formato de archivo de OneNote.

```csharp
public enum FileFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Unknown | `0` | Formato de archivo desconocido. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote en línea. |

### Ejemplos

Muestra cómo verificar si la carga de un documento falla porque el formato de OneNote 2007 no es compatible.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### Ver también

* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


