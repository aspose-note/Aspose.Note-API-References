---
title: ImageSaveOptions.Quality
second_title: Aspose.Note for .NET API リファレンス
description: ImageSaveOptions 財産. 保存された画像の品質を決定する値を取得または設定します. この値は System.Drawing.Imaging.Encoder.Quality パラメータとしてコーデックに渡されます.
type: docs
weight: 40
url: /ja/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

保存された画像の品質を決定する値を取得または設定します. この値は System.Drawing.Imaging.Encoder.Quality パラメータとしてコーデックに渡されます.

```csharp
public int Quality { get; set; }
```

### 備考

品質カテゴリの有用な値の範囲は 0 から 100 です. 指定された数値が小さいほど、圧縮率が高くなり、したがって画像の品質が低下します. 0 は最低品質の画像を提供し、100 は最高品質の画像を提供します。 . デフォルト値は 90 です。

### 例

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

JPEG 圧縮を使用してドキュメントを Tiff 形式の画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// ドキュメントを保存します。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### 関連項目

* class [ImageSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../imagesaveoptions/)
* 組み立て [Aspose.Note](../../../)


