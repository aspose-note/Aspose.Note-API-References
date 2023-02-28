---
title: Enum FileFormat
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.FileFormat enum. Rappresenta il formato file OneNote.
type: docs
weight: 90
url: /it/net/aspose.note/fileformat/
---
## FileFormat enumeration

Rappresenta il formato file OneNote.

```csharp
public enum FileFormat
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Unknown | `0` | Formato file sconosciuto. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

### Esempi

Mostra come verificare se il caricamento di un documento non è riuscito perché il formato OneNote 2007 non è supportato.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


