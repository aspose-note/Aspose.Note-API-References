---
title: HtmlSaveOptions.FontFaceTypes
second_title: Aspose.Note per .NET API Reference
description: HtmlSaveOptions proprietà. Ottiene o imposta i tipi di caratteri.
type: docs
weight: 80
url: /it/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

Ottiene o imposta i tipi di caratteri.

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Valore della proprietà

I tipi di caratteri.

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

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../htmlsaveoptions/)
* assemblea [Aspose.Note](../../../)


