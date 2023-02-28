---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note for .NET API リファレンス
description: PdfSaveOptions 財産. PDF ドキュメント内の JPEG 画像の品質を決定する値を取得または設定します 値は 0 から 100 までの範囲で変化する場合があります0 は最悪の品質ですが最大の圧縮率を意味し100 は最高の品質ですが最小の圧縮率を意味します.
type: docs
weight: 30
url: /ja/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

PDF ドキュメント内の JPEG 画像の品質を決定する値を取得または設定します。 値は 0 から 100 までの範囲で変化する場合があります。0 は最悪の品質ですが最大の圧縮率を意味し、100 は最高の品質ですが最小の圧縮率を意味します.

```csharp
public int JpegQuality { get; set; }
```

### 備考

デフォルト値は 90 です。

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

* class [PdfSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 組み立て [Aspose.Note](../../../)


