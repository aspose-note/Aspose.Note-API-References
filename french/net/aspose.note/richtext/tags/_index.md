---
title: RichText.Tags
second_title: Référence de l'API Aspose.Note pour .NET
description: RichText propriété. Obtient la liste de toutes les balises dun paragraphe.
type: docs
weight: 90
url: /fr/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Obtient la liste de toutes les balises d'un paragraphe.

```csharp
public List<ITag> Tags { get; }
```

### Exemples

Montre comment accéder aux détails des tâches Outlook.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tasks();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Itérer à travers chaque nœud
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Récupérer les propriétés
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Voir également

* interface [ITag](../../itag/)
* class [RichText](../)
* espace de noms [Aspose.Note](../../richtext/)
* Assemblée [Aspose.Note](../../../)


