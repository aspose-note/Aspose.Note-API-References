---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note for .NET API リファレンス
description: DocumentFontsSubsystem 方法. 指定されたストリームのフォントをデフォルトとして使用して新しい DocumentFontsSubsystem インスタンスを作成します
type: docs
weight: 50
url: /ja/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

指定されたストリームのフォントをデフォルトとして使用して、新しい DocumentFontsSubsystem インスタンスを作成します。

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| defaultFontStream | Stream | デフォルトのフォント名を含むストリーム。 |
| fontsSubstitutions | Dictionary`2 | フォントの置換. |

### 戻り値

[`DocumentFontsSubsystem`](../).

### 例

ストリームから既定のフォントを使用してドキュメントを pdf 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// ドキュメントを PDF として保存
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### 関連項目

* class [DocumentFontsSubsystem](../)
* 名前空間 [Aspose.Note.Fonts](../../documentfontssubsystem/)
* 組み立て [Aspose.Note](../../../)


