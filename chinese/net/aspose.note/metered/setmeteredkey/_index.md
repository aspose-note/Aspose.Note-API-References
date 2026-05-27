---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Note for .NET API 参考"
description: "Metered 方法。设置计量公钥和私钥"
type: docs
weight: 30
url: /zh/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

设置计量的公钥和私钥。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| publicKey | String | 公钥。 |
| privateKey | String | 私钥。 |

## 备注

如果您购买了计量许可证，应在应用程序启动时调用此 API，通常这就足够了。然而，如果计量在 24 小时内未能上传消费数据，许可证将被设置为评估状态。为避免这种情况，您应定期检查许可证状态；如果是评估状态，请再次调用此 API。

## 示例

展示如何设置计量许可证。

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子项
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### 另请参阅

* class [Metered](../)
* namespace [Aspose.Note](../../metered/)
* assembly [Aspose.Note](../../../)


