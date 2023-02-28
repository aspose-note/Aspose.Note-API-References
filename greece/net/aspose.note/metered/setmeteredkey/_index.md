---
title: Metered.SetMeteredKey
second_title: Aspose.Note for .NET API Reference
description: Metered μέθοδος. Ορίζει μετρημένα δημόσια και ιδιωτικά κλειδιά.
type: docs
weight: 30
url: /el/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ορίζει μετρημένα δημόσια και ιδιωτικά κλειδιά.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| publicKey | String | Το δημόσιο κλειδί. |
| privateKey | String | Το ιδιωτικό κλειδί. |

### Παρατηρήσεις

Εάν αγοράσετε μετρημένη άδεια, αυτό το API θα πρέπει να καλείται κατά την εκκίνηση της εφαρμογής, κανονικά, αυτό είναι αρκετό. Ωστόσο, εάν το metered δεν ανεβάσει δεδομένα κατανάλωσης κατά τη διάρκεια 24 ωρών, η άδεια χρήσης θα οριστεί σε κατάσταση αξιολόγησης. Για να αποφύγετε μια τέτοια περίπτωση, θα πρέπει να ελέγχετε τακτικά την κατάσταση της άδειας Εάν είναι κατάσταση αξιολόγησης, καλέστε ξανά αυτό το API.

### Παραδείγματα

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

* class [Metered](../)
* χώρος ονομάτων [Aspose.Note](../../metered/)
* συνέλευση [Aspose.Note](../../../)


