---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Fonts.DocumentFontsSubsystem クラス. Aspose.Note.Fonts.FontsSubsystem の単純な実装検索するFontFamilyOS. からのオブジェクト
type: docs
weight: 100
url: /ja/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Aspose.Note.Fonts.FontsSubsystem の単純な実装。検索するFontFamilyOS. からのオブジェクト

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | の新しいインスタンスを初期化します`DocumentFontsSubsystem`class. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | の新しいインスタンスを初期化します`DocumentFontsSubsystem`class. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | の新しいインスタンスを初期化します`DocumentFontsSubsystem`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | 静的な既定のインスタンスを取得または設定します。 |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | デフォルトのフォントを取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | 指定されたデフォルトのフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。 |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | 指定したファイルのフォントをデフォルトとして使用して、新しい DocumentFontsSubsystem インスタンスを作成します。 |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | 指定されたストリームのフォントをデフォルトとして使用して、新しい DocumentFontsSubsystem インスタンスを作成します。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | フォントを追加します。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | フォントを追加します。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | フォントを追加します。 |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | フォントの置換を追加します。 |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | フォント ファミリを取得します。 |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | 指定したフォルダーからすべての TrueType フォントを内部コレクションに読み込みます。 |

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

* class [FontsSubsystem](../fontssubsystem/)
* 名前空間 [Aspose.Note.Fonts](../../aspose.note.fonts/)
* 組み立て [Aspose.Note](../../)


