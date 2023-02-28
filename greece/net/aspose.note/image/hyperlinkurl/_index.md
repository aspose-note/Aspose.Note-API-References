---
title: Image.HyperlinkUrl
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει ή ορίζει την υπερσύνδεση που σχετίζεται με την εικόνα.
type: docs
weight: 110
url: /el/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Λαμβάνει ή ορίζει την υπερ-σύνδεση που σχετίζεται με την εικόνα.

```csharp
public string HyperlinkUrl { get; set; }
```

### Παραδείγματα

Δείχνει πώς να συνδέσετε μια υπερσύνδεση σε μια εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### Δείτε επίσης

* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


