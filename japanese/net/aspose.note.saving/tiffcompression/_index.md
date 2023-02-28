---
title: Enum TiffCompression
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.TiffCompression 列挙. ドキュメントを TIFF 形式で保存するときに使用する圧縮の種類を指定します
type: docs
weight: 880
url: /ja/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

ドキュメントを TIFF 形式で保存するときに使用する圧縮の種類を指定します。

```csharp
public enum TiffCompression
```

### 値

| 名前 | 価値 | 説明 |
| --- | --- | --- |
| None | `1` | 圧縮なしを指定します。 |
| Rle | `2` | RLE 圧縮を指定します。 |
| Ccitt3 | `3` | CCITT グループ 3 ファックス エンコーディングを指定します。 |
| Ccitt4 | `4` | CCITT グループ 4 ファックス エンコーディングを指定します。 |
| Lzw | `5` | LZW 圧縮を指定します。 |
| PackBits | `32773` | Macintosh RLE 圧縮を指定します。 |
| Jpeg | `7` | JPEG DCT 圧縮圧縮を指定します。 |

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

* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


