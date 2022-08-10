---
title: AttachedFile
second_title: Référence de l'API Aspose.Note pour .NET
description: Représente un fichier joint.
type: docs
weight: 10
url: /fr/net/aspose.note/attachedfile/
---
## AttachedFile class

Représente un fichier joint.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [AttachedFile](attachedfile#constructor)() | Initialise une nouvelle instance du[`AttachedFile`](../attachedfile) classe. |
| [AttachedFile](attachedfile#constructor_6)(string, Stream) | Initialise une nouvelle instance du[`AttachedFile`](../attachedfile) classe. |
| [AttachedFile](attachedfile#constructor_7)(string, Stream, ImageFormat) | Initialise une nouvelle instance du[`AttachedFile`](../attachedfile) classe. |
| [AttachedFile](attachedfile#constructor_8)(string, Stream, Stream, ImageFormat) | Initialise une nouvelle instance du[`AttachedFile`](../attachedfile) classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment) { get; set; } | Obtient ou définit l'alignement. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription) { get; set; } | Obtient ou définit un corps un texte alternatif pour l'icône du fichier joint. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle) { get; set; } | Obtient ou définit un titre de texte alternatif pour l'icône du fichier joint. |
| [Bytes](../../aspose.note/attachedfile/bytes) { get; } | Obtient les données binaires d'un fichier intégré. |
| [Document](../../aspose.note/node/document) { get; } | Obtient le document du nœud. |
| [Extension](../../aspose.note/attachedfile/extension) { get; } | Obtient l'extension d'un fichier intégré. |
| [FileName](../../aspose.note/attachedfile/filename) { get; } | Obtient le nom du fichier intégré. |
| [FilePath](../../aspose.note/attachedfile/filepath) { get; } | Obtient le chemin d'accès au fichier d'origine. |
| [Height](../../aspose.note/attachedfile/height) { get; } | Obtient la hauteur d'origine de l'icône du fichier intégré. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset) { get; set; } | Obtient ou définit le décalage horizontal. |
| [Icon](../../aspose.note/attachedfile/icon) { get; } | Obtient les données binaires de l'icône associée au fichier intégré. |
| [IconExtension](../../aspose.note/attachedfile/iconextension) { get; } | Obtient l'extension de l'icône. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Obtient une valeur indiquant si ce nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout) { get; set; } | Obtient ou définit une valeur indiquant si la vue du fichier est imprimée. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser) { get; set; } | Obtient ou définit une valeur indiquant si la valeur de la taille de l'icône a été explicitement mise à jour par l'utilisateur. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime) { get; set; } | Obtient ou définit l'heure de la dernière modification. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight) { get; set; } | Obtient ou définit la hauteur maximale pour afficher l'icône du fichier intégré. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth) { get; set; } | Obtient ou définit la largeur maximale pour afficher l'icône du fichier intégré. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Obtient le type de nœud. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |
| [Tags](../../aspose.note/attachedfile/tags) { get; } | Obtient la liste de toutes les balises d'un paragraphe. |
| [Text](../../aspose.note/attachedfile/text) { get; set; } | Obtient ou définit la représentation textuelle du fichier incorporé. La chaîne NE DOIT PAS contenir de caractères de la valeur 10 (saut de ligne) ou 13 (retour chariot). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset) { get; set; } | Obtient ou définit le décalage vertical. |
| [Width](../../aspose.note/attachedfile/width) { get; } | Obtient la largeur d'origine de l'icône du fichier intégré. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept)(DocumentVisitor) | Accepte le visiteur du nœud. |

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

Montre comment ajouter un fichier à un document en utilisant filepath.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialise l'objet de classe AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Ajouter un fichier joint
outlineElem.AppendChildLast(attachedFile);

// Ajoute un nœud d'élément de contour
outline.AppendChildLast(outlineElem);

// Ajoute un nœud de contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Montre comment ajouter un fichier d'un flux à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initialise l'objet de classe AttachedFile et transmet également son chemin d'accès à l'icône
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Ajouter un fichier joint
    outlineElem.AppendChildLast(attachedFile);
}

// Ajoute un nœud d'élément de contour
outline.AppendChildLast(outlineElem);

// Ajoute un nœud de contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Voir également

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
