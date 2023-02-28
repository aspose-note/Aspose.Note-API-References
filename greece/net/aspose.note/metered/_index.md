---
title: Class Metered
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Metered τάξη. Παρέχει μεθόδους για να ορίσετε μετρημένο κλειδί.
type: docs
weight: 350
url: /el/net/aspose.note/metered/
---
## Metered class

Παρέχει μεθόδους για να ορίσετε μετρημένο κλειδί.

```csharp
public class Metered
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Metered](metered/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Καταργεί την προηγούμενη άδεια εγκατάστασης. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Ορίζει μετρημένα δημόσια και ιδιωτικά κλειδιά. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Λαμβάνει πίστωση κατανάλωσης. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Λαμβάνει μέγεθος αρχείου κατανάλωσης. |

### Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει μια προσπάθεια να οριστεί το μετρημένο δημόσιο και ιδιωτικό κλειδί

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

Δείχνει πώς να ορίσετε μετρημένη άδεια.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


