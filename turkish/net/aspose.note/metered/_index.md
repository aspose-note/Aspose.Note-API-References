---
title: Class Metered
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Metered sınıf. Ölçülen anahtarı ayarlamak için yöntemler sağlar.
type: docs
weight: 350
url: /tr/net/aspose.note/metered/
---
## Metered class

Ölçülen anahtarı ayarlamak için yöntemler sağlar.

```csharp
public class Metered
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Önceki kurulum lisansını kaldırır. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Tarifeli genel ve özel anahtarları ayarlar. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Tüketim kredisi alır. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Tüketim dosyası boyutunu alır. |

### Örnekler

Bu örnekte, ölçülü genel ve özel anahtar ayarlanmaya çalışılacaktır.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

Tarifeli lisansın nasıl ayarlanacağını gösterir.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin ve ilk çocuğu alın           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Ayrıca bakınız

* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


