---
title: Document.FileFormat
second_title: Référence de l'API Aspose.Note pour .NET
description: Document propriété. Obtient le format de fichier OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /fr/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Obtient le format de fichier (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Exemples

Montre comment obtenir le format de fichier d'un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Traiter OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Traiter OneNote en ligne
        break;
}
```

### Voir également

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


