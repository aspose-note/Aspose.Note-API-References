---
title: Notebook
second_title: Référence de l'API Aspose.Note pour .NET
description: Représente un carnet Aspose.Note.
type: docs
weight: 390
url: /fr/net/aspose.note/notebook/
---
## Notebook class

Représente un carnet Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Notebook](notebook#constructor)() | Initialise une nouvelle instance du[`Notebook`](../notebook) classe. |
| [Notebook](notebook#constructor_1)(Stream) | Initialise une nouvelle instance du[`Notebook`](../notebook) class. Ouvre un bloc-notes OneNote existant à partir d'un flux. |
| [Notebook](notebook#constructor_3)(string) | Initialise une nouvelle instance du[`Notebook`](../notebook) class. Ouvre un bloc-notes OneNote existant à partir d'un fichier. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | Initialise une nouvelle instance du[`Notebook`](../notebook) class. Ouvre un bloc-notes OneNote existant à partir d'un flux. Permet de spécifier des options de chargement supplémentaires. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | Initialise une nouvelle instance du[`Notebook`](../notebook)class. Ouvre un bloc-notes OneNote existant à partir d'un fichier. Permet de spécifier des options supplémentaires telles qu'une stratégie de chargement des enfants ("paresseux"/instantané). |

## Propriétés

| Nom | La description |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Obtient ou définit la couleur. |
| [Count](../../aspose.note/notebook/count) { get; } | Obtient le nombre d'éléments contenus dans le[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Obtient ou définit le nom d'affichage. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Obtient le format de fichier (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Obtient l'identifiant global unique de l'objet. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Obtient ou définit une valeur indiquant si l'historique est activé. |
| [Item](../../aspose.note/notebook/item) { get; } | Obtient le nœud enfant du bloc-notes par l'index donné. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Ajoute le nœud à la fin de la liste. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Obtenir tous les nœuds enfants par le type de nœud. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Renvoie un énumérateur qui parcourt les nœuds enfants du[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un flux. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un fichier. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un flux. Permet de spécifier des options de chargement supplémentaires. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un fichier. Permet de spécifier des options de chargement supplémentaires. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | Ajoute un nœud de bloc-notes enfant. Ouvre un bloc-notes OneNote existant à partir d'un flux. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | Ajoute un nœud de bloc-notes enfant. Ouvre un bloc-notes OneNote existant à partir d'un fichier. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Ajoute un nœud de bloc-notes enfant. Ouvre un bloc-notes OneNote existant à partir d'un flux. Permet de spécifier des options de chargement supplémentaires. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | Ajoute un nœud de bloc-notes enfant. Ouvre un bloc-notes OneNote existant à partir d'un fichier. Permet de spécifier des options de chargement supplémentaires. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Supprime le nœud enfant. |
| [Save](../../aspose.note/notebook/save#save)(Stream) | Enregistre le document OneNote dans un flux. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | Enregistre le document OneNote dans un fichier. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | Enregistre le document OneNote dans un flux à l'aide des options d'enregistrement spécifiées. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | Enregistre le document OneNote dans un flux au format spécifié. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | Enregistre le document OneNote dans un fichier à l'aide des options d'enregistrement spécifiées. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | Enregistre le document OneNote dans un fichier au format spécifié. |

### Exemples

Montre comment enregistrer le bloc-notes.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Enregistrer le bloc-notes
notebook.Save(dataDir);
```

Montre comment enregistrer un cahier au format pdf.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Enregistrer le bloc-notes
notebook.Save(dataDir);
```

Montre comment enregistrer le bloc-notes en tant qu'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Enregistrer le bloc-notes
notebook.Save(dataDir);
```

Montre comment obtenir tout le texte d'un bloc-notes.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

Montre comment enregistrer un cahier aplati au format pdf.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Enregistrer le bloc-notes
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Montre comment parcourir les documents d'un bloc-notes en les chargeant paresseusement.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Par défaut, le chargement des enfants est "paresseux".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Le chargement réel du document enfant ne se produit qu'ici.
    // Faire quelque chose avec le document enfant
}
```

Montre comment ajouter une nouvelle section à un bloc-notes.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Ajoute un nouvel enfant au Notebook
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Enregistrer le bloc-notes
notebook.Save(dataDir);
```

Montre comment charger un bloc-notes à partir d'un flux.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Montre comment créer un bloc-notes chiffré.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Montre comment enregistrer le bloc-notes en tant qu'image avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Enregistrer le bloc-notes
notebook.Save(dataDir, notebookSaveOptions);
```

Montre comment enregistrer un cahier aplati en tant qu'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Enregistrer le bloc-notes
notebook.Save(dataDir, notebookSaveOptions);
```

Montre comment supprimer une section d'un bloc-notes.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Parcourt ses nœuds enfants pour rechercher l'élément enfant souhaité
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Supprimer l'élément enfant du bloc-notes
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Enregistrer le bloc-notes
notebook.Save(dataDir);
```

Montre comment parcourir les documents préchargés d'un bloc-notes.

```csharp
// Par défaut, le chargement des enfants est "paresseux".
// Donc pour le chargement instantané a eu lieu,
// il est nécessaire de définir l'indicateur NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Tous les documents enfants sont déjà chargés.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Faire quelque chose avec le document enfant
}
```

Montre comment passer à travers le contenu d'un bloc-notes.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Faire quelque chose avec le document enfant
        }
        else if (notebookChildNode is Notebook)
        {
            // Faire quelque chose avec le cahier enfant
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Voir également

* interface [INotebookChildNode](../inotebookchildnode)
* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
