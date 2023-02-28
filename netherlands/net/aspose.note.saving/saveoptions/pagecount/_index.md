---
title: SaveOptions.PageCount
second_title: Aspose.Note voor .NET API-referentie
description: SaveOptions eigendom. Haalt het aantal op te slaan paginas op of stelt het in. Standaard isMaxValue wat betekent dat alle paginas van het document worden weergegeven.
type: docs
weight: 20
url: /nl/net/aspose.note.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Haalt het aantal op te slaan pagina's op of stelt het in. Standaard isMaxValue wat betekent dat alle pagina's van het document worden weergegeven.

```csharp
public int PageCount { get; set; }
```

### Voorbeelden

Laat zien hoe u een document opslaat in pdf-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Stel de pagina-index in van de eerste pagina die moet worden opgeslagen
                              PageIndex = 0,

                              // Stel het aantal pagina's in
                              PageCount = 1,
                          };

// Sla het document op als PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Laat zien hoe u een document in pdf-formaat kunt opslaan met behulp van specifieke instellingen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Gebruik JPEG-compressie
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kwaliteit voor JPEG-compressie
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Laat zien hoe u een document maakt en opslaat in een opgegeven paginabereik in html-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer OneNote-document
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Opslaan in HTML-formaat
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

### Zie ook

* class [SaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../saveoptions/)
* montage [Aspose.Note](../../../)


