---
title: Metered.SetMeteredKey
second_title: Aspose.Note voor .NET API-referentie
description: Metered methode. Stelt gemeten openbare en privésleutels in.
type: docs
weight: 30
url: /nl/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Stelt gemeten openbare en privésleutels in.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| publicKey | String | De openbare sleutel. |
| privateKey | String | De privésleutel. |

### Opmerkingen

Als u een gemeten licentie aanschaft, moet deze API worden aangeroepen bij het opstarten van de applicatie, normaal gesproken is dit voldoende. Als Metered er echter niet in slaagt om verbruiksgegevens te uploaden gedurende een periode van 24 uur, wordt de licentie ingesteld op de evaluatiestatus. Om dergelijke gevallen te voorkomen, moet u regelmatig de licentiestatus controleren. Als het de evaluatiestatus is, roept u deze API opnieuw op.

### Voorbeelden

Laat zien hoe u een licentie met licentie instelt.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Zie ook

* class [Metered](../)
* naamruimte [Aspose.Note](../../metered/)
* montage [Aspose.Note](../../../)


