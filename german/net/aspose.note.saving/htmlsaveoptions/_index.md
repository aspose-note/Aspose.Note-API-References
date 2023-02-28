---
title: Class HtmlSaveOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.HtmlSaveOptions klas. Ermöglicht die Angabe zusätzlicher Optionen beim Speichern des Dokuments im HTMLFormat.
type: docs
weight: 700
url: /de/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Ermöglicht die Angabe zusätzlicher Optionen beim Speichern des Dokuments im HTML-Format.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Ruft ab oder legt fest, ob die StyleSheet-Datei für jede neue Seite separat generiert wird. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Ruft den Callback ab oder legt ihn fest, der aufgerufen wird, um eine Ressource zum Speichern von CSS zu erstellen. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Generierung von Dokumenten pro Seite aktiviert ist. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Ruft ab oder legt fest, wie CSS exportiert wird. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Ruft ab oder legt fest, wie Schriftarten exportiert werden. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Ruft ab oder legt fest, wie Bilder exportiert werden. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Ruft die Schriftarttypen ab oder legt sie fest. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Ruft den Callback ab oder legt ihn fest, der aufgerufen wird, um eine Ressource zum Speichern von Schriftarten zu erstellen. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Ruft die beim Speichern zu verwendenden Schrifteinstellungen ab oder legt sie fest |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Ruft den Callback ab oder legt ihn fest, der aufgerufen wird, um eine Ressource zum Speichern des Bildes zu erstellen. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. Standardmäßig istMaxValue , was bedeutet, dass alle Seiten des Dokuments gerendert werden. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Ruft den Callback ab oder legt ihn fest, der aufgerufen wird, um eine Ressource zum Speichern der Seite zu erstellen. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Ruft das Format ab, in dem das Dokument gespeichert ist. |

### Beispiele

Zeigt, wie ein Dokument im HTML-Format gespeichert wird, wobei alle Ressourcen (css/fonts/images) in separaten Dateien gespeichert werden.

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

Zeigt, wie ein Dokument in einem Stream im HTML-Format mit Einbettung aller Ressourcen (css/fonts/images) gespeichert wird.

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

Zeigt, wie man ein Dokument erstellt und einen bestimmten Seitenbereich im HTML-Format speichert.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Im HTML-Format speichern
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Zeigt, wie ein Dokument im HTML-Format gespeichert wird, wobei alle Ressourcen (css/fonts/images) mithilfe von benutzerdefinierten Rückrufen gespeichert werden.

```csharp
// Der folgende Code erstellt den Ordner „documentFolder“ mit document.html, den Ordner „css“ mit der Datei „style.css“, den Ordner „images“ mit Bildern und den Ordner „fonts“ mit Schriftarten.
// Die Datei „style.css“ enthält am Ende die folgende Zeichenfolge „/* Diese Zeile wird vom Benutzer manuell an den Stream angehängt */“
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

### Siehe auch

* class [SaveOptions](../saveoptions/)
* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


