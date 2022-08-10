---
title: DocumentVisitor
second_title: Référence de l'API Aspose.Note pour .NET
description: La classe abstraite pour parcourir le sous-arbre avec la racine au nœud spécifié.
type: docs
weight: 70
url: /fr/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

La classe abstraite pour parcourir le sous-arbre avec la racine au nœud spécifié.

```csharp
public abstract class DocumentVisitor
```

## Méthodes

| Nom | La description |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend)(AttachedFile) | Fin pour visiter le[`AttachedFile`](../attachedfile) nœud. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart)(AttachedFile) | Commencez à visiter le[`AttachedFile`](../attachedfile) nœud. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend)(Document) | Fin pour visiter le[`Document`](../document) nœud. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart)(Document) | Commencez à visiter le[`Document`](../document) nœud. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend)(Image) | Fin pour visiter le[`Image`](../image) nœud. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart)(Image) | Commencez à visiter le[`Image`](../image) nœud. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend)(OutlineElement) | Fin pour visiter le[`OutlineElement`](../outlineelement) nœud. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart)(OutlineElement) | Commencez à visiter le[`OutlineElement`](../outlineelement) nœud. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend)(Outline) | Fin pour visiter le[`Outline`](../outline) nœud. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend)(OutlineGroup) | Fin pour visiter le[`OutlineGroup`](../outlinegroup) nœud. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart)(OutlineGroup) | Commencez à visiter le[`OutlineGroup`](../outlinegroup) nœud. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart)(Outline) | Commencez à visiter le[`Outline`](../outline) nœud. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend)(Page) | Fin pour visiter le[`Page`](../page) nœud. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart)(Page) | Commencez à visiter le[`Page`](../page) nœud. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend)(RichText) | Fin pour visiter le[`RichText`](../richtext) nœud. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart)(RichText) | Commencez à visiter le[`RichText`](../richtext) nœud. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend)(TableCell) | Fin pour visiter le[`TableCell`](../tablecell) nœud. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart)(TableCell) | Commencez à visiter le[`TableCell`](../tablecell) nœud. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend)(Table) | Fin pour visiter le[`Table`](../table) nœud. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend)(TableRow) | Fin pour visiter le[`TableRow`](../tablerow) nœud. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart)(TableRow) | Commencez à visiter le[`TableRow`](../tablerow) nœud. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart)(Table) | Commencez à visiter le[`Table`](../table) nœud. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend)(Title) | Fin pour visiter le[`Title`](../title) nœud. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart)(Title) | Commencez à visiter le[`Title`](../title) nœud. |

### Exemples

Montre comment accéder au contenu d'un document à l'aide de visiteur.

```csharp
public static void Run()
{
    // Le chemin d'accès au répertoire des documents.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Ouvre le document que nous voulons convertir.
    Document doc = new Document(dataDir + "Aspose.one");

    // Crée un objet qui hérite de la classe DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Il s'agit du modèle de visiteur bien connu. Obtenez le modèle pour accepter un visiteur.
    // Le modèle va itérer sur lui-même en appelant les méthodes correspondantes
    // sur l'objet visiteur (c'est ce qu'on appelle visiter).
    //
    // Notez que chaque nœud dans le modèle d'objet a la méthode Accept donc la visite
    // peut être exécuté non seulement pour l'ensemble du document, mais pour n'importe quel nœud du document.
    doc.Accept(myConverter);

    // Une fois la visite terminée, on peut récupérer le résultat de l'opération,
    // qui, dans cet exemple, s'est accumulé dans le visiteur.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Implémentation simple de l'enregistrement d'un document au format texte brut. Implémenté en tant que visiteur.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// Obtient le texte brut du document qui a été accumulé par le visiteur.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Ajoute du texte à la sortie actuelle. Honore le drapeau de sortie activé/désactivé.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Appelé lorsqu'un nœud RichText est rencontré dans le document.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Appelé lorsqu'un nœud Document est rencontré dans le document.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Appelé lorsqu'un nœud Page est rencontré dans le document.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Appelé lorsque le traitement d'un nœud Page est terminé.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Appelé lorsqu'un nœud Title est rencontré dans le document.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Appelé lorsqu'un nœud Image est rencontré dans le document.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Appelé lorsqu'un nœud OutlineGroup est rencontré dans le document.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Appelé lorsqu'un nœud Outline est rencontré dans le document.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Appelé lorsqu'un nœud OutlineElement est rencontré dans le document.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Obtient le nombre total de nœuds par le visiteur
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### Voir également

* espace de noms [Aspose.Note](../../aspose.note)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
