---
title: Image.AlternativeTextTitle
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για την εικόνα.
type: docs
weight: 40
url: /el/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για την εικόνα.

```csharp
public string AlternativeTextTitle { get; set; }
```

### Παραδείγματα

Δείχνει πώς να ορίσετε την περιγραφή κειμένου για μια εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
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

### Δείτε επίσης

* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


