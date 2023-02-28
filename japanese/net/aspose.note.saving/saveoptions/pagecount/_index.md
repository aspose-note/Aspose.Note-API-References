---
title: SaveOptions.PageCount
second_title: Aspose.Note for .NET API リファレンス
description: SaveOptions 財産. 保存するページ数を取得または設定しますデフォルトではMaxValue はドキュメントのすべてのページがレンダリングされることを意味します.
type: docs
weight: 20
url: /ja/net/aspose.note.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

保存するページ数を取得または設定します。デフォルトではMaxValue は、ドキュメントのすべてのページがレンダリングされることを意味します.

```csharp
public int PageCount { get; set; }
```

### 例

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

### 関連項目

* class [SaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../saveoptions/)
* 組み立て [Aspose.Note](../../../)


