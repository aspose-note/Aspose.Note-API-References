---
title: HtmlSaveOptions.ImageSavingCallback
second_title: Aspose.Note für .NET-API-Referenz
description: HtmlSaveOptions eigendom. Ruft den Callback ab oder legt ihn fest der aufgerufen wird um eine Ressource zum Speichern des Bildes zu erstellen.
type: docs
weight: 100
url: /de/net/aspose.note.saving/htmlsaveoptions/imagesavingcallback/
---
## HtmlSaveOptions.ImageSavingCallback property

Ruft den Callback ab oder legt ihn fest, der aufgerufen wird, um eine Ressource zum Speichern des Bildes zu erstellen.

```csharp
public IImageSavingCallback ImageSavingCallback { get; set; }
```

### Beispiele

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

* interface [IImageSavingCallback](../../../aspose.note.saving.html/iimagesavingcallback/)
* class [HtmlSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../htmlsaveoptions/)
* Montage [Aspose.Note](../../../)


