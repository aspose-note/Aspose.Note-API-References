---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note for .NET API リファレンス
description: DocumentFontsSubsystem 方法. 指定したファイルのフォントをデフォルトとして使用して新しい DocumentFontsSubsystem インスタンスを作成します
type: docs
weight: 40
url: /ja/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

指定したファイルのフォントをデフォルトとして使用して、新しい DocumentFontsSubsystem インスタンスを作成します。

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | デフォルトのフォント名を含むファイル。 |
| fontsSubstitutions | Dictionary`2 | フォントの置換. |

### 戻り値

[`DocumentFontsSubsystem`](../).

### 例

ファイルからデフォルトのフォントを使用してドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// ドキュメントを PDF として保存
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### 関連項目

* class [DocumentFontsSubsystem](../)
* 名前空間 [Aspose.Note.Fonts](../../documentfontssubsystem/)
* 組み立て [Aspose.Note](../../../)


