---
title: License.SetLicense
second_title: Aspose.Note for .NET API Reference
description: License μέθοδος. Παρέχει άδεια χρήσης του στοιχείου.
type: docs
weight: 20
url: /el/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Παρέχει άδεια χρήσης του στοιχείου.

```csharp
public void SetLicense(string licenseName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| licenseName | String | Μπορεί να είναι ένα πλήρες ή σύντομο όνομα αρχείου ή όνομα ενός ενσωματωμένου πόρου. Χρησιμοποιήστε μια κενή συμβολοσειρά για να μεταβείτε στη λειτουργία αξιολόγησης. |

### Παρατηρήσεις

Προσπαθεί να βρει την άδεια στις ακόλουθες τοποθεσίες:

1. Ρητή διαδρομή.

2. Ο φάκελος που περιέχει τη διάταξη του στοιχείου Aspose.

3. Ο φάκελος που περιέχει τη συγκρότηση κλήσης του πελάτη.

4. Ο φάκελος που περιέχει τη διάταξη καταχώρησης (εκκίνησης).

5. Ένας ενσωματωμένος πόρος στη διάταξη κλήσης του πελάτη.

**Σημείωση:**Στο .NET Compact Framework, προσπαθεί να βρει την άδεια χρήσης μόνο σε αυτές τις τοποθεσίες:

1. Ρητή διαδρομή.

2. Ένας ενσωματωμένος πόρος στη διάταξη κλήσης του πελάτη.

### Παραδείγματα

Δείχνει πώς να φορτώσετε μια άδεια χρήσης για το Aspose.Note από ένα αρχείο.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Δείχνει πώς να φορτώσετε μια άδεια χρήσης για το Aspose.Note από ενσωματωμένο πόρο αρχείου.

```csharp
// Δημιουργήστε την κλάση άδειας χρήσης
Aspose.Note.License license = new Aspose.Note.License();

// Περάστε μόνο το όνομα του αρχείου άδειας χρήσης που είναι ενσωματωμένο στη συγκρότηση
license.SetLicense("Aspose.Note.lic");
```

### Δείτε επίσης

* class [License](../)
* χώρος ονομάτων [Aspose.Note](../../license/)
* συνέλευση [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Παρέχει άδεια χρήσης του στοιχείου.

```csharp
public void SetLicense(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Μια ροή που περιέχει την άδεια. |

### Παρατηρήσεις

Χρησιμοποιήστε αυτήν τη μέθοδο για να φορτώσετε μια άδεια από μια ροή.

### Παραδείγματα

Δείχνει πώς να φορτώσετε μια άδεια για το Aspose.Note από μια ροή.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Δείτε επίσης

* class [License](../)
* χώρος ονομάτων [Aspose.Note](../../license/)
* συνέλευση [Aspose.Note](../../../)


