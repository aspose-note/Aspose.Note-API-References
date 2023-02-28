---
title: Metered.SetMeteredKey
second_title: Aspose.Note per .NET API Reference
description: Metered metodo. Imposta chiavi pubbliche e private misurate.
type: docs
weight: 30
url: /it/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Imposta chiavi pubbliche e private misurate.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| publicKey | String | La chiave pubblica. |
| privateKey | String | La chiave privata. |

### Osservazioni

Se acquisti una licenza a consumo, questa API dovrebbe essere richiamata all'avvio dell'applicazione, normalmente è sufficiente. Tuttavia, se il contatore non riesce a caricare i dati di consumo durante il periodo di 24 ore, la licenza verrà impostata sullo stato di valutazione. Per evitare questo caso, dovresti controllare regolarmente lo stato della licenza. Se si tratta di uno stato di valutazione, chiama di nuovo questa API.

### Esempi

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

* class [Metered](../)
* spazio dei nomi [Aspose.Note](../../metered/)
* assemblea [Aspose.Note](../../../)


