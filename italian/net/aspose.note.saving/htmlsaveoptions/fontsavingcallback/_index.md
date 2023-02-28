---
title: HtmlSaveOptions.FontSavingCallback
second_title: Aspose.Note per .NET API Reference
description: HtmlSaveOptions proprietà. Ottiene o imposta il callback chiamato per creare una risorsa per archiviare il carattere.
type: docs
weight: 90
url: /it/net/aspose.note.saving/htmlsaveoptions/fontsavingcallback/
---
## HtmlSaveOptions.FontSavingCallback property

Ottiene o imposta il callback chiamato per creare una risorsa per archiviare il carattere.

```csharp
public IFontSavingCallback FontSavingCallback { get; set; }
```

### Esempi

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

* interface [IFontSavingCallback](../../../aspose.note.saving.html/ifontsavingcallback/)
* class [HtmlSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../htmlsaveoptions/)
* assemblea [Aspose.Note](../../../)


