---
title: Class HtmlSaveOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.HtmlSaveOptions classe. Consente di specificare opzioni aggiuntive durante il salvataggio del documento in formato HTML.
type: docs
weight: 700
url: /it/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Consente di specificare opzioni aggiuntive durante il salvataggio del documento in formato HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Ottiene o imposta se il file StyleSheet verrà generato separatamente per ogni nuova pagina. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Ottiene o imposta il callback che viene chiamato per creare la risorsa per memorizzare CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Ottiene o imposta un valore che indica se è abilitata la generazione di documenti per pagina. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Ottiene o imposta il modo in cui il css viene esportato. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Ottiene o imposta la modalità di esportazione dei caratteri. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Ottiene o imposta la modalità di esportazione delle immagini. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Ottiene o imposta i tipi di caratteri. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Ottiene o imposta il callback chiamato per creare una risorsa per archiviare il carattere. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Ottiene o imposta le impostazioni del carattere da utilizzare durante il salvataggio |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Ottiene o imposta il callback chiamato per creare una risorsa per archiviare l'immagine. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. Per impostazione predefinita èMaxValue che significa che verranno visualizzate tutte le pagine del documento. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice della prima pagina da salvare. Di default è 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Ottiene o imposta il callback che viene chiamato per creare la risorsa per archiviare la pagina. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Ottiene il formato in cui viene salvato il documento. |

### Esempi

Mostra come salvare un documento in formato html memorizzando tutte le risorse (css/font/immagini) in file separati.

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

Mostra come salvare un documento in uno stream in formato html con l'incorporamento di tutte le risorse (css/font/immagini).

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

Mostra come creare un documento e salvarlo in un intervallo di pagine specificato in formato html.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inizializza il documento OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Stile predefinito per tutto il testo nel documento.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Salva in formato HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Mostra come salvare un documento in formato html con l'archiviazione di tutte le risorse (css/caratteri/immagini) utilizzando i callback definiti dall'utente.

```csharp
// Il codice seguente crea la cartella "documentFolder" contenente document.html, la cartella "css" con il file "style.css", la cartella "images" con le immagini e la cartella "fonts" con i caratteri.
// Il file 'style.css' conterrà alla fine la seguente stringa "/* Questa riga viene aggiunta allo streaming manualmente dall'utente */"
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

### Guarda anche

* class [SaveOptions](../saveoptions/)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


