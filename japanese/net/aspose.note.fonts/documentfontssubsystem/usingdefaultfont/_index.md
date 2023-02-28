---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note for .NET API リファレンス
description: DocumentFontsSubsystem 方法. 指定されたデフォルトのフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します
type: docs
weight: 30
url: /ja/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

指定されたデフォルトのフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| defaultFontName | String | デフォルトのフォント名. |
| fontsSubstitutions | Dictionary`2 | フォントの置換. |

### 戻り値

[`DocumentFontsSubsystem`](../).

### 例

指定された既定のフォントを使用してドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// ドキュメントを PDF として保存
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### 関連項目

* class [DocumentFontsSubsystem](../)
* 名前空間 [Aspose.Note.Fonts](../../documentfontssubsystem/)
* 組み立て [Aspose.Note](../../../)


