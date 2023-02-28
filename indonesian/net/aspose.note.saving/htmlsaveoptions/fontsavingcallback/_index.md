---
title: HtmlSaveOptions.FontSavingCallback
second_title: Aspose.Note untuk Referensi .NET API
description: HtmlSaveOptions Properti. Mendapat atau menyetel panggilan balik yang dipanggil untuk membuat sumber daya untuk menyimpan font.
type: docs
weight: 90
url: /id/net/aspose.note.saving/htmlsaveoptions/fontsavingcallback/
---
## HtmlSaveOptions.FontSavingCallback property

Mendapat atau menyetel panggilan balik yang dipanggil untuk membuat sumber daya untuk menyimpan font.

```csharp
public IFontSavingCallback FontSavingCallback { get; set; }
```

### Contoh

Menunjukkan cara menyimpan dokumen dalam format html dengan menyimpan semua sumber daya (css/font/gambar) dengan menggunakan panggilan balik yang ditentukan pengguna.

```csharp
// Kode di bawah membuat folder 'documentFolder' yang berisi document.html, folder 'css' dengan file 'style.css', folder 'images' dengan gambar dan folder 'fonts' dengan font.
// File 'style.css' akan berisi string berikut "/* Baris ini ditambahkan untuk streaming secara manual oleh pengguna */"
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

### Lihat juga

* interface [IFontSavingCallback](../../../aspose.note.saving.html/ifontsavingcallback/)
* class [HtmlSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../htmlsaveoptions/)
* perakitan [Aspose.Note](../../../)


