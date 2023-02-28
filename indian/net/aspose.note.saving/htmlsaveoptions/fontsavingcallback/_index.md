---
title: HtmlSaveOptions.FontSavingCallback
second_title: Aspose.Note .NET API संदर्भ के लिए
description: HtmlSaveOptions संपत्त. उस कलबैक क प्रप्त य सेट करत है जसे फ़न्ट स्टर करने के लए संसधन बनने के लए कह जत है
type: docs
weight: 90
url: /hi/net/aspose.note.saving/htmlsaveoptions/fontsavingcallback/
---
## HtmlSaveOptions.FontSavingCallback property

उस कॉलबैक को प्राप्त या सेट करता है जिसे फ़ॉन्ट स्टोर करने के लिए संसाधन बनाने के लिए कहा जाता है।

```csharp
public IFontSavingCallback FontSavingCallback { get; set; }
```

### उदाहरण

उपयोगकर्ता परिभाषित कॉलबैक का उपयोग कर सभी संसाधनों (सीएसएस/फोंट/छवियों) को संग्रहीत करने के साथ एचटीएमएल प्रारूप में दस्तावेज़ को कैसे सहेजना दिखाता है।

```csharp
// नीचे दिया गया कोड 'documentFolder' फोल्डर बनाता है जिसमें document.html, 'css' फोल्डर 'style.css' फाइल के साथ, 'इमेज' फोल्डर इमेज के साथ और 'फोंट' फोल्डर फॉन्ट के साथ होता है।
// 'style.css' फ़ाइल में अंत में निम्न स्ट्रिंग होगी "/* यह लाइन उपयोगकर्ता द्वारा मैन्युअल रूप से स्ट्रीम करने के लिए जोड़ी गई है */"
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

### यह सभी देखें

* interface [IFontSavingCallback](../../../aspose.note.saving.html/ifontsavingcallback/)
* class [HtmlSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../htmlsaveoptions/)
* सभा [Aspose.Note](../../../)


