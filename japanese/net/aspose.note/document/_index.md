---
title: Class Document
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Document クラス. Aspose.Note ドキュメントを表します
type: docs
weight: 60
url: /ja/net/aspose.note/document/
---
## Document class

Aspose.Note ドキュメントを表します。

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Document](document/#constructor)() | の新しいインスタンスを初期化します`Document` class. 空の OneNote ドキュメントを作成します。 |
| [Document](document/#constructor_1)(Stream) | の新しいインスタンスを初期化します`Document` class. ストリームから既存の OneNote ドキュメントを開きます。 |
| [Document](document/#constructor_3)(string) | の新しいインスタンスを初期化します`Document` class. ファイルから既存の OneNote ドキュメントを開きます。 |
| [Document](document/#constructor_2)(Stream, LoadOptions) | の新しいインスタンスを初期化します`Document` class. ストリームから既存の OneNote ドキュメントを開きます。暗号化パスワードなどの追加オプションを指定できます。 |
| [Document](document/#constructor_4)(string, LoadOptions) | の新しいインスタンスを初期化します`Document`class. ファイルから既存の OneNote ドキュメントを開きます。暗号化パスワードなどの追加オプションを指定できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | Aspose.Note がレイアウト変更の検出を自動的に実行するかどうかを示す値を取得または設定します。 デフォルト値は`真実`. |
| [Color](../../aspose.note/document/color/) { get; set; } | 色を取得または設定します。 |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | 作成時刻を取得または設定します。 |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | 表示名を取得または設定します。 |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | ファイル形式を取得します (OneNote 2010、OneNote Online). |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | オブジェクトのグローバルに一意な ID を取得します。 |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | 前回の変更以降にドキュメント レイアウトに加えられたすべての変更を検出します。[`DetectLayoutChanges`](./detectlayoutchanges/) call. の場合[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/)ドキュメント エクスポートの開始時に自動的に使用される、true に設定します。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | を取得します[`PageHistory`](../pagehistory/)これには、ドキュメントに表示された各ページの完全な履歴が含まれています (最も古いインデックス 0). 現在のページのリビジョンには、次のようにアクセスできます。[`Current`](../pagehistory/current/)履歴バージョンのコレクションとは別に含まれています. |
| [Import](../../aspose.note/document/import/#import)(Stream, PdfImportOptions, MergeOptions) | 提供された PDF ドキュメントから一連のページをインポートします。 |
| [Import](../../aspose.note/document/import/#import_1)(string, PdfImportOptions, MergeOptions) | 提供された PDF ドキュメントから一連のページをインポートします。 |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | 一連のページをドキュメントに結合します。 |
| [Print](../../aspose.note/document/print/#print)() | デフォルトのプリンターを使用してドキュメントを印刷します。 |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | デフォルトのプリンターを使用してドキュメントを印刷します。 |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | OneNote ドキュメントをストリームに保存します。 |
| [Save](../../aspose.note/document/save/#save_3)(string) | OneNote ドキュメントをファイルに保存します。 |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | 指定した形式で OneNote ドキュメントをストリームに保存します。 |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | 指定された保存オプションを使用して、OneNote ドキュメントをストリームに保存します。 |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | 指定した形式で OneNote ドキュメントをファイルに保存します。 |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | 指定された保存オプションを使用して、OneNote ドキュメントをファイルに保存します。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | ストリームからのドキュメントが暗号化されているかどうかを確認します。 確認するには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | ファイルのドキュメントが暗号化されているかどうかをチェックします。 チェックするには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | ストリームからのドキュメントが暗号化されているかどうかを確認します。 確認するには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | ストリームからのドキュメントが暗号化されているかどうかを確認します。 確認するには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | ファイルのドキュメントが暗号化されているかどうかをチェックします。 チェックするには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | ファイルのドキュメントが暗号化されているかどうかをチェックします。 チェックするには、このドキュメントを完全にロードする必要があります。したがって、この方法ではパフォーマンスが低下する可能性があります. |

### 例

標準の Windows ダイアログとデフォルト オプションを使用して、ドキュメントをプリンタに送信する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

ドキュメントを保存する方法を示します。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

ドキュメントを暗号化する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

ドキュメントを暗号化して保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

SaveFormat 列挙体を使用してドキュメントを保存する方法を示します。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

OneSaveOptions を使用してドキュメントを保存する方法を示します。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

ドキュメントのページ数を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// ページ数を取得
int count = oneFile.Count();

// 出力画面にカウントを出力
Console.WriteLine(count);
```

デフォルト設定を使用してドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// ドキュメントを PDF として保存
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

ドキュメントを gif 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// ドキュメントを gif として保存します。
oneFile.Save(dataDir, SaveFormat.Gif);
```

文書を JPEG 形式の画像として保存するときの画質を設定する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// ドキュメントを保存します。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

ドキュメントを画像として保存するときに画像の解像度を設定する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// ドキュメントを保存します。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

ドキュメントのファイル形式を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010 の処理
        break;
    case FileFormat.OneNoteOnline:
        // OneNote をオンラインで処理する
        break;
}
```

ハイパーリンクを画像にバインドする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

ドキュメントをストリームに保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// ストリームの位置をゼロに巻き戻し、次のリーダーの準備が整うようにします。
dstStream.Seek(0, SeekOrigin.Begin);
```

ドキュメントがパスワードで保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

新しいセクションをノートブックに追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Notebook に新しい子を追加します
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// ノートブックを保存します
notebook.Save(dataDir);
```

OneNote 2007 形式がサポートされていないためにドキュメントの読み込みが失敗したかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

ページの以前のバージョンを復元する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

ページを複製する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込む
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 履歴なしで新しいドキュメントにクローンします
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// 履歴付きの新しいドキュメントにクローンします
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

画像のテキスト説明を設定する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

ページに関するメタ情報を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

長い OneNote ページを pdf 形式で保存すると、複数のページに分割されます。このサンプルは、ページの区切りにあるオブジェクトの分割ロジックを構成する方法を示しています。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

ドキュメントを png 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions オブジェクトを初期化します 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // ページのインデックスを設定
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// ドキュメントを PNG として保存します。
oneFile.Save(dataDir, opts);
```

ページの履歴を編集する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

ドキュメントが特定のパスワードによってパスワード保護されているかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

ドキュメントにダーク テーマ スタイルを適用する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

ノートブックのコンテンツを渡す方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // 子ドキュメントで何かをする
        }
        else if (notebookChildNode is Notebook)
        {
            // 子ノートブックで何かをする
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

ドキュメントから画像を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての画像ノードを取得
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 画像バイトをファイルに保存します
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

ドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions オブジェクトを初期化します
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 保存する最初のページのページ インデックスを設定します
                              PageIndex = 0,

                              // ページ数を設定
                              PageCount = 1,
                          };

// ドキュメントを PDF として保存
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

特定の設定を使用してドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions オブジェクトを初期化します
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // JPEG 圧縮を使用
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 圧縮の品質
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

オプションを指定して標準の Windows ダイアログを使用して、ドキュメントをプリンターに送信する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

添付ファイルのコンテンツを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Sample1.one");

// 添付ファイル ノードのリストを取得します
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// すべてのノードを繰り返します
foreach (AttachedFile file in nodes)
{
    // ストリームオブジェクトに添付ファイルをロード
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // ローカル ファイルを作成します
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // ファイルストリームをコピー
            CopyStream(outputStream, fileStream);
        }
    }
}
```

画像のメタ情報を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての画像ノードを取得
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

ページの履歴を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込む
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 最初のページを取得
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

filepath を使用してドキュメントにファイルを追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile クラス オブジェクトを初期化します
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// 添付ファイルを追加
outlineElem.AppendChildLast(attachedFile);

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

ドキュメントを作成し、デフォルト オプションを使用して HTML 形式で保存する方法を示します。

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

ページが競合ページ (つまり、OneNote が自動的にマージできなかった変更がある) であるかどうかを確認する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込む
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // デフォルトでは、競合ページは保存時にスキップされます。
    // 非競合としてマークすると、通常の履歴として保存されます。
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

ユーザー定義のプロパティを使用して、ファイルからドキュメントに画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// ストリームからドキュメントを読み込みます。
Document doc = new Document(dataDir + "Aspose.one");

// ドキュメントの最初のページを取得します。
Aspose.Note.Page page = doc.FirstChild;

// ファイルから画像を読み込みます。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 必要に応じて画像のサイズを変更します (オプション)。
                              Width = 100,
                              Height = 100,

                              // ページ内の画像の位置を設定します (オプション)。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 画像の配置を設定
                              Alignment = HorizontalAlignment.Right
                          };

// ページに画像を追加します。
page.AppendChildLast(image);
```

ストリームからドキュメントにファイルを追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // AttachedFile クラス オブジェクトを初期化し、そのアイコン パスも渡します
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 添付ファイルを追加
    outlineElem.AppendChildLast(attachedFile);
}

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

長い OneNote ページを pdf 形式で保存すると、複数のページに分割されます。この例は、ページの区切りにあるオブジェクトの分割ロジックを構成する方法を示しています。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
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

タイトル付きのページを持つドキュメントを作成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document クラスのオブジェクトを作成します
Document doc = new Aspose.Note.Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// ドキュメント内のすべてのテキストのデフォルト スタイル。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// ページ タイトルのプロパティを設定します
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// ドキュメントに Page ノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

ストリームからドキュメントに画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // イメージ名、拡張子、およびストリームを使用して 2 番目のイメージをロードします。
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 画像の配置を設定
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

ファイルからドキュメントに画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトを初期化し、オフセット プロパティを設定します
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// ファイル パスで画像を読み込みます。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 画像の配置を設定
                              Alignment = HorizontalAlignment.Right
                          };

// 画像を追加
outlineElem.AppendChildLast(image);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem);

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

テキストを含むドキュメントを作成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Page page = new Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle クラス オブジェクトを初期化し、書式設定プロパティを設定します
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText クラス オブジェクトを初期化し、テキスト スタイルを適用します
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText ノードを追加
outlineElem.AppendChildLast(text);

// OutlineElement ノードを追加
outline.AppendChildLast(outlineElem);

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

ドキュメントをさまざまな形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 新しいドキュメントを初期化します
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 新しいページを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// ドキュメント内のすべてのテキストのデフォルト スタイル。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントをさまざまな形式で保存し、テキストのフォント サイズを設定し、レイアウトの変更を手動で検出します。
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

ハイパーリンクをテキストにバインドする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tasks();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem);

// タイトル クラス オブジェクトを初期化します
Title title = new Title() { TitleText = titleText };

// Page クラス オブジェクトを初期化します
Page page = new Note.Page() { Title = title };

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

ビジターを使用してドキュメントのコンテンツにアクセスする方法を示します。

```csharp
public static void Run()
{
    /// ドキュメント ディレクトリへのパス。
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    /// 変換するドキュメントを開きます。
    Document doc = new Document(dataDir + "Aspose.one");

    /// DocumentVisitor クラスから継承するオブジェクトを作成します。
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    /// これはよく知られている Visitor パターンです。訪問者を受け入れるモデルを取得します。
    /// モデルは、対応するメソッドを呼び出すことによってそれ自体を反復処理します
    /// 訪問者オブジェクト (これは訪問と呼ばれます)。
    ///
    /// オブジェクト モデルのすべてのノードに Accept メソッドがあることに注意してください。
    /// ドキュメント全体だけでなく、ドキュメント内の任意のノードに対して実行できます。
    doc.Accept(myConverter);

    /// 訪問が完了すると、操作の結果を取得できます。
    /// この例では、訪問者に蓄積されています。
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

//// <summary>
//// ドキュメントをプレーン テキスト形式で保存する単純な実装。ビジターとして実装されます。
//// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    //// <summary>
    //// 訪問者が蓄積したドキュメントの平文を取得します。
    //// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    //// <summary>
    //// 現在の出力にテキストを追加します。有効化/無効化された出力フラグを尊重します。
    //// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    //// <summary>
    //// ドキュメント内で RichText ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    //// <summary>
    //// ドキュメント内で Document ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で Page ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    //// <summary>
    //// Page ノードの処理が終了したときに呼び出されます。
    //// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    //// <summary>
    //// ドキュメント内で Title ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で Image ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で OutlineGroup ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で Outline ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で OutlineElement ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    //// <summary>
    //// 訪問者によるノードの総数を取得します
    //// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### 関連項目

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


