---
title: HtmlSaveOptions.FontFaceTypes
second_title: Aspose.Note for .NET API リファレンス
description: HtmlSaveOptions 財産. フォント フェイス タイプを取得または設定します
type: docs
weight: 80
url: /ja/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

フォント フェイス タイプを取得または設定します。

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### プロパティ値

フォント フェースの種類。

### 例

すべてのリソース (css/fonts/images) を別のファイルに保存して、ドキュメントを HTML 形式で保存する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

すべてのリソース (css/fonts/images) を埋め込んで、ドキュメントを HTML 形式でストリームに保存する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

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

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 組み立て [Aspose.Note](../../../)


