---
title: AttachedFile.Bytes
second_title: Référence de l'API Aspose.Note pour .NET
description: AttachedFile propriété. Obtient les données binaires dun fichier intégré.
type: docs
weight: 50
url: /fr/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Obtient les données binaires d'un fichier intégré.

```csharp
public byte[] Bytes { get; }
```

### Exemples

Montre comment obtenir le contenu d'un fichier joint.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Attachments();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Obtenir une liste des nœuds de fichiers joints
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Itérer sur tous les nœuds
foreach (AttachedFile file in nodes)
{
    // Charger le fichier joint dans un objet stream
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Créer un fichier local
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copie le flux du fichier
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Voir également

* class [AttachedFile](../)
* espace de noms [Aspose.Note](../../attachedfile/)
* Assemblée [Aspose.Note](../../../)


