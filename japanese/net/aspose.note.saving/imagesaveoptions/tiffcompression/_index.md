---
title: ImageSaveOptions.TiffCompression
second_title: Aspose.Note for .NET API リファレンス
description: ImageSaveOptions 財産. 生成された画像を TIFF 形式で保存するときに使用する圧縮の種類を取得または設定します
type: docs
weight: 60
url: /ja/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

生成された画像を TIFF 形式で保存するときに使用する圧縮の種類を取得または設定します。

```csharp
public TiffCompression TiffCompression { get; set; }
```

### 例

PackBits 圧縮を使用してドキュメントを Tiff 形式の画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// ドキュメントを保存します。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
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

CCITT Group 3 ファックス圧縮を使用して、ドキュメントを Tiff 形式の画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// ドキュメントを保存します。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### 関連項目

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../imagesaveoptions/)
* 組み立て [Aspose.Note](../../../)


