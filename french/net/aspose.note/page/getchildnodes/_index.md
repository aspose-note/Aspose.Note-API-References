---
title: Page.GetChildNodes
second_title: Référence de l'API Aspose.Note pour .NET
description: Page méthode. Obtenir tous les nœuds enfants de la page par le type de nœud.
type: docs
weight: 150
url: /fr/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Obtenir tous les nœuds enfants de la page par le type de nœud.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Paramètre | La description |
| --- | --- |
| T1 | Type d'éléments dans la liste renvoyée. |

### Return_Value

Une liste de nœuds enfants.

### Exemples

Montre comment obtenir tout le texte du document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupérer le texte
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Affiche le texte sur l'écran de sortie
Console.WriteLine(text);
```

Montre comment obtenir tout le texte de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère la liste des nœuds de la page
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Récupérer le texte
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Affiche le texte sur l'écran de sortie
    Console.WriteLine(text);
}
```

Montre comment parcourir toutes les pages et effectuer un remplacement dans le texte.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Remplace le texte d'une forme
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Enregistrer dans n'importe quel format de fichier pris en charge
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Montre comment parcourir le texte de la page et effectuer un remplacement.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Récupère tous les nœuds RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Remplace le texte d'une forme
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Enregistrer dans n'importe quel format de fichier pris en charge
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Voir également

* interface [INode](../../inode/)
* class [Page](../)
* espace de noms [Aspose.Note](../../page/)
* Assemblée [Aspose.Note](../../../)


