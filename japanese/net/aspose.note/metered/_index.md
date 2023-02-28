---
title: Class Metered
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Metered クラス. メータリング キーを設定するメソッドを提供します
type: docs
weight: 350
url: /ja/net/aspose.note/metered/
---
## Metered class

メータリング キーを設定するメソッドを提供します。

```csharp
public class Metered
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Metered](metered/)() | デフォルトのコンストラクター。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | 以前にセットアップしたライセンスを削除します。 |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | 従量制の公開鍵と秘密鍵を設定します。 |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | 消費クレジットを取得します。 |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | 消費ファイルサイズを取得します。 |

### 例

この例では、従量制の公開鍵と秘密鍵を設定しようとします

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

従量制ライセンスの設定方法を示します。

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


