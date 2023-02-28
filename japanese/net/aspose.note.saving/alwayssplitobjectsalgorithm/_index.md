---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm クラス. オブジェクトが元のページに収まらない場合に備えてオブジェクトをいくつかの部分に分割します
type: docs
weight: 550
url: /ja/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

オブジェクトが元のページに収まらない場合に備えて、オブジェクトをいくつかの部分に分割します。

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | デフォルトのコンストラクター。 |

### 例

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

### 関連項目

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


