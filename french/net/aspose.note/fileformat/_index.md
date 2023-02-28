---
title: Enum FileFormat
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.FileFormat énumération. Représente le format de fichier OneNote.
type: docs
weight: 90
url: /fr/net/aspose.note/fileformat/
---
## FileFormat enumeration

Représente le format de fichier OneNote.

```csharp
public enum FileFormat
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| Unknown | `0` | Format de fichier inconnu. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote en ligne. |

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

* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


