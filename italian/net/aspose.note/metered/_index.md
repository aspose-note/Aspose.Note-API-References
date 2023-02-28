---
title: Class Metered
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Metered classe. Fornisce metodi per impostare la chiave misurata.
type: docs
weight: 350
url: /it/net/aspose.note/metered/
---
## Metered class

Fornisce metodi per impostare la chiave misurata.

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered/)() | Default_Costruttore |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Rimuove la licenza precedentemente configurata. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Imposta chiavi pubbliche e private misurate. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Ottiene credito a consumo. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Ottiene la dimensione del file di consumo. |

### Esempi

In questo esempio, verrà effettuato un tentativo di impostare la chiave pubblica e privata misurata

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

Mostra come impostare la licenza a consumo.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote e ottieni il primo figlio           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Guarda anche

* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


