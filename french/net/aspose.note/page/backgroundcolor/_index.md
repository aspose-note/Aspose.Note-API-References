---
title: Page.BackgroundColor
second_title: Référence de l'API Aspose.Note pour .NET
description: Page propriété. Obtient ou définit la couleur darrièreplan de la page.
type: docs
weight: 30
url: /fr/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Obtient ou définit la couleur d'arrière-plan de la page.

```csharp
public Color BackgroundColor { get; set; }
```

### Exemples

Montre comment définir la couleur d'arrière-plan de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote et obtenir le premier enfant           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
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

### Voir également

* class [Page](../)
* espace de noms [Aspose.Note](../../page/)
* Assemblée [Aspose.Note](../../../)


