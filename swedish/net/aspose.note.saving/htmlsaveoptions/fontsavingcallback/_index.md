---
title: HtmlSaveOptions.FontSavingCallback
second_title: Aspose.Note för .NET API-referens
description: HtmlSaveOptions fast egendom. Hämtar eller ställer in återuppringningen som anropas för att skapa resurs för att lagra teckensnitt.
type: docs
weight: 90
url: /sv/net/aspose.note.saving/htmlsaveoptions/fontsavingcallback/
---
## HtmlSaveOptions.FontSavingCallback property

Hämtar eller ställer in återuppringningen som anropas för att skapa resurs för att lagra teckensnitt.

```csharp
public IFontSavingCallback FontSavingCallback { get; set; }
```

### Exempel

Visar hur man sparar ett dokument i html-format med lagring av alla resurser (css/fonts/images) genom att använda användardefinierade callbacks.

```csharp
// Koden nedan skapar 'documentFolder'-mappen som innehåller document.html, 'css'-mappen med 'style.css'-filen, 'images'-mappen med bilder och 'fonts'-mappen med typsnitt.
// 'style.css'-filen kommer att innehålla i slutet följande sträng "/* Denna rad har lagts till för att streama manuellt av användaren */"
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

### Se även

* interface [IFontSavingCallback](../../../aspose.note.saving.html/ifontsavingcallback/)
* class [HtmlSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../htmlsaveoptions/)
* hopsättning [Aspose.Note](../../../)


