---
title: SetMeteredKey
second_title: Aspose.Note för .NET API-referens
description: Ställer in mätta offentliga och privata nycklar.
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
| publicKey | String | Den offentliga nyckeln. |
| privateKey | String | Den privata nyckeln. |

### Anmärkningar

Om du köper mätlicens bör detta API anropas vid start av applikationen, normalt räcker detta. Men om mätt misslyckas med att ladda upp förbrukningsdata under 24 timmar kommer licensen att ställas in på utvärderingsstatus. För att undvika sådana fall bör du regelbundet kontrollera licensstatusen Om det är utvärderingsstatus, anropa detta API igen.

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

* class [Metered](../../metered)
* namnutrymme [Aspose.Note](../../metered)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->