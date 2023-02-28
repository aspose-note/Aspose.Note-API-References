---
title: HtmlSaveOptions.ImageSavingCallback
second_title: .NET API 참조용 Aspose.Note
description: HtmlSaveOptions 재산. 이미지를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져오거나 설정합니다.
type: docs
weight: 100
url: /ko/net/aspose.note.saving/htmlsaveoptions/imagesavingcallback/
---
## HtmlSaveOptions.ImageSavingCallback property

이미지를 저장할 리소스를 생성하기 위해 호출되는 콜백을 가져오거나 설정합니다.

```csharp
public IImageSavingCallback ImageSavingCallback { get; set; }
```

### 예

사용자 정의 콜백을 사용하여 모든 리소스(css/fonts/images)를 저장하여 html 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 아래 코드는 document.html이 포함된 'documentFolder' 폴더, 'style.css' 파일이 포함된 'css' 폴더, 이미지가 포함된 'images' 폴더, 글꼴이 포함된 'fonts' 폴더를 생성합니다.
// 'style.css' 파일은 끝에 다음 문자열을 포함합니다. "/* 이 줄은 사용자가 수동으로 스트림에 추가합니다 */"
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

### 또한보십시오

* interface [IImageSavingCallback](../../../aspose.note.saving.html/iimagesavingcallback/)
* class [HtmlSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 집회 [Aspose.Note](../../../)


