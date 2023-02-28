---
title: Document.Print
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. デフォルトのプリンターを使用してドキュメントを印刷します
type: docs
weight: 130
url: /ja/net/aspose.note/document/print/
---
## Print() {#print}

デフォルトのプリンターを使用してドキュメントを印刷します。

```csharp
public void Print()
```

### 例

標準の Windows ダイアログとデフォルト オプションを使用して、ドキュメントをプリンタに送信する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

オプションを指定して標準の Windows ダイアログを使用して、ドキュメントをプリンターに送信する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

デフォルトのプリンターを使用してドキュメントを印刷します。

```csharp
public void Print(PrintOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| options | PrintOptions | ドキュメントの印刷に使用されるオプション。 null にすることができます。 |

### 関連項目

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


