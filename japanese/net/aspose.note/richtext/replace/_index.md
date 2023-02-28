---
title: RichText.Replace
second_title: Aspose.Note for .NET API リファレンス
description: RichText 方法. このインスタンスで出現する指定された Unicode 文字をすべて指定された別の Unicode 文字に置き換えます
type: docs
weight: 200
url: /ja/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

このインスタンスで出現する指定された Unicode 文字をすべて、指定された別の Unicode 文字に置き換えます。

```csharp
public RichText Replace(char oldChar, char newChar)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| oldChar | Char | 古い char. |
| newChar | Char | 新しい char. |

### 戻り値

[`RichText`](../).

### 関連項目

* class [RichText](../)
* 名前空間 [Aspose.Note](../../richtext/)
* 組み立て [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

現在のインスタンス内の指定された文字列のすべてのオカレンスを別の指定された文字列に置き換えます。

```csharp
public RichText Replace(string oldValue, string newValue)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| oldValue | String | 古い値. |
| newValue | String | 新しい値。 |

### 戻り値

[`RichText`](../).

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 例

ページのテキストを通過させて置換する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// すべての RichText ノードを取得します
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 図形のテキストを置き換える
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// サポートされている任意のファイル形式に保存
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

テンプレート内の特殊なテキスト部分を置き換えて新しいドキュメントを生成する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// テンプレート ドキュメントを Aspose.Note にロードします。
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// すべてのテンプレート単語を置き換えましょう
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### 関連項目

* class [RichText](../)
* 名前空間 [Aspose.Note](../../richtext/)
* 組み立て [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

現在のインスタンスで出現する指定された文字列をすべて、指定されたスタイルの別の指定された文字列に置き換えます。

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| oldValue | String | 古い値. |
| newValue | String | 新しい値。 |
| style | TextStyle | 新しい値のスタイル. |

### 戻り値

[`RichText`](../).

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 関連項目

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* 名前空間 [Aspose.Note](../../richtext/)
* 組み立て [Aspose.Note](../../../)


