---
title: TextStyle.HyperlinkAddress
second_title: Aspose.Note for .NET API Reference
description: TextStyle ιδιοκτησία. Λαμβάνει ή ορίζει τη διεύθυνση υπερσύνδεσης. Πρέπει να οριστεί εάν η τιμή τουIsHyperlink Η ιδιότητα είναι αληθής.
type: docs
weight: 60
url: /el/net/aspose.note/textstyle/hyperlinkaddress/
---
## TextStyle.HyperlinkAddress property

Λαμβάνει ή ορίζει τη διεύθυνση υπερσύνδεσης. Πρέπει να οριστεί εάν η τιμή του[`IsHyperlink`](../ishyperlink/) Η ιδιότητα είναι αληθής.

```csharp
public string HyperlinkAddress { get; set; }
```

### Παραδείγματα

Δείχνει πώς να συνδέσετε μια υπερ-σύνδεση σε ένα κείμενο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tasks();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
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

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem);

// Αρχικοποίηση αντικειμένου κλάσης τίτλου
Title title = new Title() { TitleText = titleText };

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Page page = new Note.Page() { Title = title };

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Δείτε επίσης

* class [TextStyle](../)
* χώρος ονομάτων [Aspose.Note](../../textstyle/)
* συνέλευση [Aspose.Note](../../../)


