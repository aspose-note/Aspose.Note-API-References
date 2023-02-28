---
title: Class Document
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Document classe. Représente un document Aspose.Note.
type: docs
weight: 60
url: /fr/net/aspose.note/document/
---
## Document class

Représente un document Aspose.Note.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Document](document/#constructor)() | Initialise une nouvelle instance du`Document` class. Crée un document OneNote vierge. |
| [Document](document/#constructor_1)(Stream) | Initialise une nouvelle instance du`Document` class. Ouvre un document OneNote existant à partir d'un flux. |
| [Document](document/#constructor_3)(string) | Initialise une nouvelle instance du`Document` class. Ouvre un document OneNote existant à partir d'un fichier. |
| [Document](document/#constructor_2)(Stream, LoadOptions) | Initialise une nouvelle instance du`Document` class. Ouvre un document OneNote existant à partir d'un flux. Permet de spécifier des options supplémentaires telles qu'un mot de passe de chiffrement. |
| [Document](document/#constructor_4)(string, LoadOptions) | Initialise une nouvelle instance du`Document`class. Ouvre un document OneNote existant à partir d'un fichier. Permet de spécifier des options supplémentaires telles qu'un mot de passe de chiffrement. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | Obtient ou définit une valeur indiquant si Aspose.Note effectue automatiquement la détection des modifications de mise en page. La valeur par défaut est`vrai` . |
| [Color](../../aspose.note/document/color/) { get; set; } | Obtient ou définit la couleur. |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | Obtient ou définit l'heure de création. |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | Obtient ou définit le nom d'affichage. |
| [Document](../../aspose.note/node/document/) { get; } | Obtient le document du nœud. |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | Obtient le format de fichier (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | Obtient l'identifiant global unique de l'objet. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtient le type de nœud. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | Accepte le visiteur du nœud. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | Détecte toutes les modifications apportées à la mise en page du document depuis la précédente[`DetectLayoutChanges`](./detectlayoutchanges/) appeler. Au cas où[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) défini sur vrai, utilisé automatiquement au début de l'exportation du document. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | Obtient le[`PageHistory`](../pagehistory/) qui contient l'historique complet de chaque page présentée dans un document (la plus ancienne à l'index 0). La révision de la page actuelle est accessible en tant que[`Current`](../pagehistory/current/) et contenus séparément de la collection des versions historiques. |
| [Import](../../aspose.note/document/import/#import)(Stream, PdfImportOptions, MergeOptions) | Importe un ensemble de pages à partir du document PDF fourni. |
| [Import](../../aspose.note/document/import/#import_1)(string, PdfImportOptions, MergeOptions) | Importe un ensemble de pages à partir du document PDF fourni. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | Fusionne un ensemble de pages dans le document. |
| [Print](../../aspose.note/document/print/#print)() | Imprime le document à l'aide de l'imprimante par défaut. |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | Imprime le document à l'aide de l'imprimante par défaut. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | Enregistre le document OneNote dans un flux. |
| [Save](../../aspose.note/document/save/#save_3)(string) | Enregistre le document OneNote dans un fichier. |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | Enregistre le document OneNote dans un flux au format spécifié. |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | Enregistre le document OneNote dans un flux à l'aide des options d'enregistrement spécifiées. |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | Enregistre le document OneNote dans un fichier au format spécifié. |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | Enregistre le document OneNote dans un fichier à l'aide des options d'enregistrement spécifiées. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | Vérifie si un document d'un flux est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | Vérifie si un document d'un fichier est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | Vérifie si un document d'un flux est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | Vérifie si un document d'un flux est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | Vérifie si un document d'un fichier est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | Vérifie si un document d'un fichier est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances. |

### Exemples

Montre comment envoyer un document à une imprimante à l'aide de la boîte de dialogue Windows standard avec les options par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Montre comment enregistrer un document.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Montre comment un document chiffré.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Montre comment enregistrer un document avec cryptage.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Montre comment enregistrer un document à l'aide de l'énumération SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Montre comment enregistrer un document à l'aide de OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Montre comment obtenir le nombre de pages d'un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère le nombre de pages
int count = oneFile.Count();

// Nombre d'impressions sur l'écran de sortie
Console.WriteLine(count);
```

Montre comment enregistrer un document au format pdf en utilisant les paramètres par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Montre comment enregistrer un document au format gif.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Montre comment définir une qualité d'image lors de l'enregistrement d'un document en tant qu'image au format JPEG.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Enregistre le document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Montre comment définir une résolution d'image lors de l'enregistrement d'un document en tant qu'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Enregistre le document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

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

Montre comment lier un lien hypertexte à une image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" } ;

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Montre comment enregistrer un document dans un flux.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Rembobine la position du flux à zéro pour qu'il soit prêt pour le prochain lecteur.
dstStream.Seek(0, SeekOrigin.Begin);
```

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
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

Montre comment restaurer la version précédente d'une page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote et obtenir le premier enfant           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Montre comment cloner une page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Cloner dans un nouveau document sans historique
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Cloner dans un nouveau document avec historique
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Montre comment enregistrer un document au format html en stockant toutes les ressources (css/fonts/images) dans des fichiers séparés.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Montre comment enregistrer un document dans un flux au format html avec intégration de toutes les ressources (css/fonts/images).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

Montre comment définir la description textuelle d'une image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Montre comment obtenir des méta-informations sur une page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Lorsque de longues pages OneNote sont enregistrées au format pdf, elles sont réparties sur plusieurs pages. L'exemple montre comment configurer la logique de fractionnement des objets situés sur les sauts de page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Montre comment enregistrer un document au format png.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Définir l'index de la page
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Enregistrez le document au format PNG.
oneFile.Save(dataDir, opts);
```

Montre comment modifier l'historique de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote et obtenir le premier enfant           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

Montre comment appliquer le style de thème sombre à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
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

Montre comment obtenir une image à partir d'un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds Image
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Enregistre les octets de l'image dans un fichier
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Montre comment enregistrer un document au format pdf.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Définit l'index de la première page à enregistrer
                              PageIndex = 0,

                              // Définir le nombre de pages
                              PageCount = 1,
                          };

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Montre comment enregistrer un document au format pdf en utilisant des paramètres spécifiques.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Utiliser la compression Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualité pour la compression JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Montre comment envoyer un document à une imprimante à l'aide de la boîte de dialogue Windows standard avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

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

Montre comment obtenir les méta-informations de l'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Montre comment obtenir l'historique de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Récupère la première page
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
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

Montre comment créer un document et l'enregistrer au format html à l'aide des options par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiser le document OneNote
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Enregistrer au format HTML
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Montre comment vérifier si une page est une page en conflit (c'est-à-dire qu'elle contient des modifications que OneNote n'a pas pu fusionner automatiquement).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Par défaut, les pages en conflit sont simplement ignorées lors de l'enregistrement.
    // Si vous le marquez comme non conflictuel, il sera enregistré comme d'habitude dans l'historique.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Montre comment ajouter une image d'un fichier à un document avec des propriétés définies par l'utilisateur.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document à partir du flux.
Document doc = new Document(dataDir + "Aspose.one");

// Récupère la première page du document.
Aspose.Note.Page page = doc.FirstChild;

// Charge une image à partir du fichier.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Modifiez la taille de l'image selon vos besoins (optionnel).
                              Width = 100,
                              Height = 100,

                              // Définit l'emplacement de l'image dans la page (optionnel).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Définir l'alignement de l'image
                              Alignment = HorizontalAlignment.Right
                          };

// Ajoute l'image à la page.
page.AppendChildLast(image);
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

Lorsque de longues pages OneNote sont enregistrées au format pdf, elles sont réparties sur plusieurs pages. L'exemple montre comment configurer la logique de découpage des objets situés sur les sauts de page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Montre comment créer un document et enregistrer au format html une plage de pages spécifiée.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiser le document OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Enregistrer au format HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Montre comment créer un document avec une page de titre.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crée un objet de la classe Document
Document doc = new Aspose.Note.Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Définir les propriétés du titre de la page
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Ajoute le noeud Page dans le document
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Montre comment ajouter une image du flux à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Charge la deuxième image en utilisant le nom, l'extension et le flux de l'image.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Définir l'alignement de l'image
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Montre comment ajouter une image d'un fichier à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialise l'objet de la classe Outline et définit les propriétés de décalage
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Charge une image par le chemin du fichier.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Définir l'alignement de l'image
                              Alignment = HorizontalAlignment.Right
                          };

// Ajouter une image
outlineElem.AppendChildLast(image);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem);

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Montre comment créer un document avec un texte.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Crée un objet de la classe Document
Document doc = new Document();

// Initialise l'objet de la classe Page
Page page = new Page(doc);

// Initialise l'objet de la classe Outline
Outline outline = new Outline(doc);

// Initialise l'objet de classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialise l'objet de classe TextStyle et définit les propriétés de formatage
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialise l'objet de classe RichText et applique le style de texte
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Ajouter un noeud RichText
outlineElem.AppendChildLast(text);

// Ajoute le noeud OutlineElement
outline.AppendChildLast(outlineElem);

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Montre comment enregistrer un document dans différents formats.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialise le nouveau Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialise la nouvelle Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Style par défaut pour tout le texte du document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Ajoute le nœud de la page
doc.AppendChildLast(page);

// Enregistrez le document OneNote dans différents formats, définissez la taille de la police du texte et détectez manuellement les modifications de mise en page.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Montre comment enregistrer un document au format html en stockant toutes les ressources (css/fonts/images) en utilisant des rappels définis par l'utilisateur.

```csharp
// Le code ci-dessous crée le dossier 'documentFolder' contenant document.html, le dossier 'css' avec le fichier 'style.css', le dossier 'images' avec les images et le dossier 'fonts' avec les polices.
// Le fichier 'style.css' contiendra à la fin la chaîne suivante "/* Cette ligne est ajoutée pour être diffusée manuellement par l'utilisateur */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

Montre comment lier un lien hypertexte à un texte.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crée un objet de la classe Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Ajout d'éléments de contour
outline.AppendChildLast(outlineElem);

// Initialise l'objet de la classe Titre
Title title = new Title() { TitleText = titleText };

// Initialise l'objet de la classe Page
Page page = new Note.Page() { Title = title };

// Ajouter un noeud Contour
page.AppendChildLast(outline);

// Ajouter un nœud de page
doc.AppendChildLast(page);

// Enregistrer le document OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


