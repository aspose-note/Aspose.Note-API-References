---
title: HtmlSaveOptions.ImageSavingCallback
second_title: Aspose.Note voor .NET API-referentie
description: HtmlSaveOptions eigendom. Haalt of stelt de callback in die wordt aangeroepen om een bron te maken om de afbeelding op te slaan.
type: docs
weight: 100
url: /nl/net/aspose.note.saving/htmlsaveoptions/imagesavingcallback/
---
## HtmlSaveOptions.ImageSavingCallback property

Haalt of stelt de callback in die wordt aangeroepen om een bron te maken om de afbeelding op te slaan.

```csharp
public IImageSavingCallback ImageSavingCallback { get; set; }
```

### Voorbeelden

Laat zien hoe u een document opslaat in html-indeling met opslag van alle bronnen (css/fonts/afbeeldingen) door gebruik te maken van door de gebruiker gedefinieerde callbacks.

```csharp
// De onderstaande code maakt de map 'documentFolder' met daarin document.html, de map 'css' met het bestand 'style.css', de map 'images' met afbeeldingen en de map 'fonts' met lettertypen.
// Het bestand 'style.css' bevat aan het einde de volgende tekenreeks "/* Deze regel is toegevoegd om handmatig door de gebruiker te streamen */"
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

### Zie ook

* interface [IImageSavingCallback](../../../aspose.note.saving.html/iimagesavingcallback/)
* class [HtmlSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../htmlsaveoptions/)
* montage [Aspose.Note](../../../)


