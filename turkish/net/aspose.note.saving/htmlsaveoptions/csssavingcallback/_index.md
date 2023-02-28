---
title: HtmlSaveOptions.CssSavingCallback
second_title: Aspose.Note for .NET API Referansı
description: HtmlSaveOptions mülk. CSSyi depolamak için kaynak oluşturmak üzere çağrılan geri aramayı alır veya ayarlar.
type: docs
weight: 30
url: /tr/net/aspose.note.saving/htmlsaveoptions/csssavingcallback/
---
## HtmlSaveOptions.CssSavingCallback property

CSS'yi depolamak için kaynak oluşturmak üzere çağrılan geri aramayı alır veya ayarlar.

```csharp
public ICssSavingCallback CssSavingCallback { get; set; }
```

### Örnekler

Kullanıcı tanımlı geri aramalar kullanarak tüm kaynakları (css/fonts/images) depolayarak bir belgenin html formatında nasıl kaydedileceğini gösterir.

```csharp
// Aşağıdaki kod, document.html'yi içeren 'documentFolder' klasörünü, 'style.css' dosyasını içeren 'css' klasörünü, resimleri içeren 'images' klasörünü ve fontları içeren 'fonts' klasörünü oluşturur.
// 'style.css' dosyası sonunda şu dizeyi içerecektir "/* Bu satır akışa kullanıcı tarafından manuel olarak eklenmiştir */"
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

### Ayrıca bakınız

* interface [ICssSavingCallback](../../../aspose.note.saving.html/icsssavingcallback/)
* class [HtmlSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../htmlsaveoptions/)
* toplantı [Aspose.Note](../../../)


