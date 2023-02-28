---
title: HtmlSaveOptions.FontSavingCallback
second_title: Aspose.Note for .NET API Reference
description: HtmlSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει την επανάκληση που καλείται να δημιουργήσει πόρο για αποθήκευση γραμματοσειράς.
type: docs
weight: 90
url: /el/net/aspose.note.saving/htmlsaveoptions/fontsavingcallback/
---
## HtmlSaveOptions.FontSavingCallback property

Λαμβάνει ή ορίζει την επανάκληση που καλείται να δημιουργήσει πόρο για αποθήκευση γραμματοσειράς.

```csharp
public IFontSavingCallback FontSavingCallback { get; set; }
```

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή html με την αποθήκευση όλων των πόρων (css/ γραμματοσειρές/εικόνες) χρησιμοποιώντας επανακλήσεις που ορίζονται από το χρήστη.

```csharp
// Ο παρακάτω κώδικας δημιουργεί φάκελο "documentFolder" που περιέχει document.html, φάκελο "css" με αρχείο "style.css", φάκελο "images" με εικόνες και φάκελο "fonts" με γραμματοσειρές.
// Το αρχείο 'style.css' θα περιέχει στο τέλος την ακόλουθη συμβολοσειρά "/* Αυτή η γραμμή προστίθεται στη ροή μη αυτόματα από τον χρήστη */"
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

### Δείτε επίσης

* interface [IFontSavingCallback](../../../aspose.note.saving.html/ifontsavingcallback/)
* class [HtmlSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../htmlsaveoptions/)
* συνέλευση [Aspose.Note](../../../)


