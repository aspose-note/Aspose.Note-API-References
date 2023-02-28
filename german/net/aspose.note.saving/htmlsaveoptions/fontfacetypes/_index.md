---
title: HtmlSaveOptions.FontFaceTypes
second_title: Aspose.Note für .NET-API-Referenz
description: HtmlSaveOptions eigendom. Ruft die Schriftarttypen ab oder legt sie fest.
type: docs
weight: 80
url: /de/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

Ruft die Schriftarttypen ab oder legt sie fest.

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Eigentumswert

Die Schriftarttypen.

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

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../htmlsaveoptions/)
* Montage [Aspose.Note](../../../)


