---
title: Class ImageBinarizationOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.ImageBinarizationOptions クラス. 画像の二値化のオプション.
type: docs
weight: 710
url: /ja/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

画像の二値化のオプション.

```csharp
public class ImageBinarizationOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | 二値化方法を取得または設定します。 デフォルト値はFixedThreshold. |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | 固定しきい値 2 値化法のしきい値を取得または設定します。 デフォルト値は 128 です。 |

### 例

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

* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


