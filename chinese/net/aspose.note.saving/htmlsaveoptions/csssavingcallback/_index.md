---
title: HtmlSaveOptions.CssSavingCallback
second_title: Aspose.Note for .NET API 参考
description: HtmlSaveOptions 财产. 获取或设置创建资源存储CSS时调用的回调
type: docs
weight: 30
url: /zh/net/aspose.note.saving/htmlsaveoptions/csssavingcallback/
---
## HtmlSaveOptions.CssSavingCallback property

获取或设置创建资源存储CSS时调用的回调。

```csharp
public ICssSavingCallback CssSavingCallback { get; set; }
```

### 例子

显示如何使用用户定义的回调以 html 格式保存文档并存储所有资源（css/字体/图像）。

```csharp
// 下面的代码创建包含 document.html 的“documentFolder”文件夹、包含“style.css”文件的“css”文件夹、包含图像的“images”文件夹和包含字体的“fonts”文件夹。
// 'style.css' 文件将在末尾包含以下字符串“/* This line is appended to stream manually by user */”
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

### 也可以看看

* interface [ICssSavingCallback](../../../aspose.note.saving.html/icsssavingcallback/)
* class [HtmlSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 部件 [Aspose.Note](../../../)


