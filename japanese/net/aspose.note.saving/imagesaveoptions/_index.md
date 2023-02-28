---
title: Class ImageSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.ImageSaveOptions クラス. ドキュメント ページを画像にレンダリングするときに追加オプションを指定できます
type: docs
weight: 720
url: /ja/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

ドキュメント ページを画像にレンダリングするときに追加オプションを指定できます。

```csharp
public class ImageSaveOptions : SaveOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | の新しいインスタンスを初期化します`ImageSaveOptions`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | 画像の 2 値化のオプションを取得または設定します。 |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | 取得または設定[`ColorMode`](./colormode/)出力画像用. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 保存中に使用されるフォントの設定を取得または設定します |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 保存するページ数を取得または設定します。デフォルトではMaxValue は、ドキュメントのすべてのページがレンダリングされることを意味します. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 保存する最初のページのインデックスを取得または設定します。デフォルトは 0. です |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | 保存された画像の品質を決定する値を取得または設定します. この値は System.Drawing.Imaging.Encoder.Quality パラメータとしてコーデックに渡されます. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | 生成された画像の解像度を 1 インチあたりのドット数で取得または設定します。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | ドキュメントの保存形式を取得します。 |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | 生成された画像を TIFF 形式で保存するときに使用する圧縮の種類を取得または設定します。 |

### 例

SaveFormat を使用してドキュメントを JPEG 形式の画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// ドキュメントを保存します。
oneFile.Save(dataDir, SaveFormat.Jpeg);
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

ImageSaveOptions を使用してドキュメントを Bmp 形式の画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// ドキュメントを保存します。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
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

ドキュメントをグレースケール イメージとして保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// ドキュメントを gif として保存します。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

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

指定したオプションを使用してノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
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

フラット化されたノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
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

大津の方法を使用してドキュメントをバイナリ イメージとして保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// ドキュメントを gif として保存します。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

固定しきい値を使用してドキュメントをバイナリ イメージとして保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// ドキュメントを gif として保存します。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### 関連項目

* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


