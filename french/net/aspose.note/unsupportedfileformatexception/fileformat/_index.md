---
title: UnsupportedFileFormatException.FileFormat
second_title: Référence de l'API Aspose.Note pour .NET
description: UnsupportedFileFormatException propriété. Obtient le format de fichier des données transmises si elles sont détectées.
type: docs
weight: 10
url: /fr/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Obtient le format de fichier des données transmises si elles sont détectées.

```csharp
public FileFormat FileFormat { get; }
```

### Exemples

Montre comment vérifier si le chargement d'un document a échoué car le format OneNote 2007 n'est pas pris en charge.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* espace de noms [Aspose.Note](../../unsupportedfileformatexception/)
* Assemblée [Aspose.Note](../../../)


