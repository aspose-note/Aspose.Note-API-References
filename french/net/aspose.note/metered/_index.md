---
title: Class Metered
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Metered classe. Fournit des méthodes pour définir la clé mesurée.
type: docs
weight: 350
url: /fr/net/aspose.note/metered/
---
## Metered class

Fournit des méthodes pour définir la clé mesurée.

```csharp
public class Metered
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## Méthodes

| Nom | La description |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Supprime la licence précédemment configurée. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Définit des clés publiques et privées mesurées. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Obtient un crédit de consommation. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Obtient la taille du fichier de consommation. |

### Exemples

Dans cet exemple, une tentative sera faite pour définir des clés publiques et privées mesurées

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

Montre comment définir une licence limitée.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote et obtenir le premier enfant           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Voir également

* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


