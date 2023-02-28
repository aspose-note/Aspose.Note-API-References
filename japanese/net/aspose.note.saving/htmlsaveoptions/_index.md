---
title: Class HtmlSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.HtmlSaveOptions クラス. ドキュメントを HTML 形式で保存するときに追加のオプションを指定できます
type: docs
weight: 700
url: /ja/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

ドキュメントを HTML 形式で保存するときに、追加のオプションを指定できます。

```csharp
public class HtmlSaveOptions : SaveOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | 新しいページごとに StyleSheet ファイルを個別に生成するかどうかを取得または設定します。 |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | CSS を格納するリソースを作成するために呼び出されるコールバックを取得または設定します。 |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | ページごとのドキュメント生成が有効かどうかを示す値を取得または設定します。 |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | css のエクスポート方法を取得または設定します。 |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | フォントのエクスポート方法を取得または設定します。 |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | 画像のエクスポート方法を取得または設定します。 |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | フォント フェイス タイプを取得または設定します。 |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | フォントを格納するリソースを作成するために呼び出されるコールバックを取得または設定します。 |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 保存中に使用されるフォントの設定を取得または設定します |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | 画像を保存するリソースを作成するために呼び出されるコールバックを取得または設定します。 |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 保存するページ数を取得または設定します。デフォルトではMaxValue は、ドキュメントのすべてのページがレンダリングされることを意味します. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 保存する最初のページのインデックスを取得または設定します。デフォルトは 0. です |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | リソースを作成してページを保存するために呼び出されるコールバックを取得または設定します。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | ドキュメントの保存形式を取得します。 |

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

ドキュメントを作成し、指定した範囲のページを html 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote ドキュメントを初期化します
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// ドキュメント内のすべてのテキストのデフォルト スタイル。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML形式で保存
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
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

* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


