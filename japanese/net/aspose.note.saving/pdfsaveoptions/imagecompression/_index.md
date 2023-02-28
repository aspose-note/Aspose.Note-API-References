---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note for .NET API リファレンス
description: PdfSaveOptions 財産. PDF ファイル内の画像に適用される圧縮の種類を取得または設定します
type: docs
weight: 20
url: /ja/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

PDF ファイル内の画像に適用される圧縮の種類を取得または設定します。

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

### 例

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

### 関連項目

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 組み立て [Aspose.Note](../../../)


