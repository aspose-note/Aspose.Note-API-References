---
title: Class Metered
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Metered klass. Tillhandahåller metoder för att ställa in mätnyckel.
type: docs
weight: 350
url: /sv/net/aspose.note/metered/
---
## Metered class

Tillhandahåller metoder för att ställa in mätnyckel.

```csharp
public class Metered
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Tar bort tidigare installationslicens. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Ställer in mätta offentliga och privata nycklar. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Får konsumtionskredit. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Får förbrukningsfilstorlek. |

### Exempel

I det här exemplet kommer ett försök att göras att ställa in mätt offentlig och privat nyckel

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

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

* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


