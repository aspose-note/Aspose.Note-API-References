---
title: HtmlSaveOptions.CssSavingCallback
second_title: Aspose.Note for .NET API リファレンス
description: HtmlSaveOptions 財産. CSS を格納するリソースを作成するために呼び出されるコールバックを取得または設定します
type: docs
weight: 30
url: /ja/net/aspose.note.saving/htmlsaveoptions/csssavingcallback/
---
## HtmlSaveOptions.CssSavingCallback property

CSS を格納するリソースを作成するために呼び出されるコールバックを取得または設定します。

```csharp
public ICssSavingCallback CssSavingCallback { get; set; }
```

### 例

ユーザー定義のコールバックを使用して、すべてのリソース (css/fonts/images) を保存してドキュメントを HTML 形式で保存する方法を示します。

```csharp
// 以下のコードは、document.html を含む「documentFolder」フォルダー、「style.css」ファイルを含む「css」フォルダー、画像を含む「images」フォルダー、およびフォントを含む「fonts」フォルダーを作成します。
// 'style.css' ファイルの末尾には、次の文字列が含まれます。"/* This line is appended to stream manual by user */"
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

### 関連項目

* interface [ICssSavingCallback](../../../aspose.note.saving.html/icsssavingcallback/)
* class [HtmlSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 組み立て [Aspose.Note](../../../)


