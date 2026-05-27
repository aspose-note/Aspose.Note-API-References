---
title: "Metered 类"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Metered 类。提供设置计量密钥的方法"
type: docs
weight: 420
url: /zh/net/aspose.note/metered/
---
## Metered class

提供设置计量密钥的方法。

```csharp
public class Metered
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Metered](metered/)() | 默认构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | 删除先前设置的许可证。 |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | 设置计量的公钥和私钥。 |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | 获取消耗积分。 |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | 获取消耗的文件大小。 |

## 示例

在此示例中，将尝试设置计量的公钥和私钥。

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


