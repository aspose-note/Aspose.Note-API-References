---
title: Metered.SetMeteredKey
second_title: Aspose.Note for .NET API Referansı
description: Metered yöntem. Tarifeli genel ve özel anahtarları ayarlar.
type: docs
weight: 30
url: /tr/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Tarifeli genel ve özel anahtarları ayarlar.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| publicKey | String | Genel anahtar. |
| privateKey | String | Özel anahtar. |

### Notlar

Eğer metered lisansı satın alırsanız, bu API'nin uygulama başlangıcında çağrılması gerekir, normalde bu yeterlidir. Ancak, metered 24 saat boyunca tüketim verilerini yükleyemezse, lisans değerlendirme durumuna geçer. Böyle bir durumla karşılaşmamak için lisans durumunu düzenli olarak kontrol etmelisiniz. Değerlendirme durumu ise bu API'yi tekrar arayın.

### Örnekler

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

* class [Metered](../)
* ad alanı [Aspose.Note](../../metered/)
* toplantı [Aspose.Note](../../../)


