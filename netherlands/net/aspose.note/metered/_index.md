---
title: Class Metered
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Metered klas. Biedt methoden om gemeten sleutel in te stellen.
type: docs
weight: 350
url: /nl/net/aspose.note/metered/
---
## Metered class

Biedt methoden om gemeten sleutel in te stellen.

```csharp
public class Metered
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Metered](metered/)() | De standaard constructeur. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Verwijdert eerder ingestelde licentie. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Stelt gemeten openbare en privésleutels in. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Krijgt consumptietegoed. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Krijgt de bestandsgrootte van het verbruik. |

### Voorbeelden

In dit voorbeeld wordt geprobeerd een gemeten openbare en privésleutel in te stellen

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

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

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


