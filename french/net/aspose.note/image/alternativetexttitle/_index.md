---
title: Image.AlternativeTextTitle
second_title: Référence de l'API Aspose.Note pour .NET
description: Image propriété. Obtient ou définit un titre de texte alternatif pour limage.
type: docs
weight: 40
url: /fr/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Obtient ou définit un titre de texte alternatif pour l'image.

```csharp
public string AlternativeTextTitle { get; set; }
```

### Exemples

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

### Voir également

* class [Image](../)
* espace de noms [Aspose.Note](../../image/)
* Assemblée [Aspose.Note](../../../)


