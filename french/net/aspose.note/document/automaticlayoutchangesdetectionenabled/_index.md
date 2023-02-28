---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Référence de l'API Aspose.Note pour .NET
description: Document propriété. Obtient ou définit une valeur indiquant si Aspose.Note effectue automatiquement la détection des modifications de mise en page. La valeur par défaut estvrai .
type: docs
weight: 20
url: /fr/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Obtient ou définit une valeur indiquant si Aspose.Note effectue automatiquement la détection des modifications de mise en page. La valeur par défaut est`vrai` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### Exemples

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

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


