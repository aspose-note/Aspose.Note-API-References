---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note per .NET API Reference
description: UnsupportedFileFormatException proprietà. Ottiene il formato file dei dati passati se rilevati.
type: docs
weight: 10
url: /it/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Ottiene il formato file dei dati passati se rilevati.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* spazio dei nomi [Aspose.Note](../../unsupportedfileformatexception/)
* assemblea [Aspose.Note](../../../)


