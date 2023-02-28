---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note for .NET API リファレンス
description: ImageBinarizationOptions 財産. 固定しきい値 2 値化法のしきい値を取得または設定します デフォルト値は 128 です
type: docs
weight: 30
url: /ja/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

固定しきい値 2 値化法のしきい値を取得または設定します。 デフォルト値は 128 です。

```csharp
public byte BinarizationThreshold { get; set; }
```

### 例

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

* class [ImageBinarizationOptions](../)
* 名前空間 [Aspose.Note.Saving](../../imagebinarizationoptions/)
* 組み立て [Aspose.Note](../../../)


