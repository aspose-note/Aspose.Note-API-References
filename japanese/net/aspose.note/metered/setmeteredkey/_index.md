---
title: Metered.SetMeteredKey
second_title: Aspose.Note for .NET API リファレンス
description: Metered 方法. 従量制の公開鍵と秘密鍵を設定します
type: docs
weight: 30
url: /ja/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

従量制の公開鍵と秘密鍵を設定します。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| publicKey | String | 公開鍵。 |
| privateKey | String | 秘密鍵。 |

### 備考

従量制ライセンスを購入した場合、この API はアプリケーションの起動時に呼び出される必要があります。通常はこれで十分です。 ただし、従量制ライセンスが 24 時間以内に消費データのアップロードに失敗した場合、ライセンスは評価ステータスに設定されます。このような事態を避けるために、ライセンスの状態を定期的に確認してください。評価状態の場合は、この API を再度呼び出してください。

### 例

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

* class [Metered](../)
* 名前空間 [Aspose.Note](../../metered/)
* 組み立て [Aspose.Note](../../../)


