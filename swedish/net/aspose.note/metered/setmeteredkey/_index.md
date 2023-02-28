---
title: Metered.SetMeteredKey
second_title: Aspose.Note för .NET API-referens
description: Metered metod. Ställer in mätta offentliga och privata nycklar.
type: docs
weight: 30
url: /sv/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ställer in mätta offentliga och privata nycklar.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| publicKey | String | Den publika nyckeln. |
| privateKey | String | Den privata nyckeln. |

### Anmärkningar

Om du köper mätlicens bör detta API anropas vid start av applikationen, normalt räcker detta. Men om mätt inte laddar upp förbrukningsdata under 24 timmar kommer licensen att ställas in på utvärderingsstatus. För att undvika sådana fall bör du regelbundet kontrollera licensstatusen Om det är utvärderingsstatus, anropa detta API igen.

### Exempel

Visar hur man ställer in mätlicens.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Se även

* class [Metered](../)
* namnutrymme [Aspose.Note](../../metered/)
* hopsättning [Aspose.Note](../../../)


