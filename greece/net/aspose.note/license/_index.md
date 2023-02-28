---
title: Class License
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.License τάξη. Παρέχει μεθόδους για την άδεια χρήσης του στοιχείου.
type: docs
weight: 310
url: /el/net/aspose.note/license/
---
## License class

Παρέχει μεθόδους για την άδεια χρήσης του στοιχείου.

```csharp
public class License
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [License](license/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Παρέχει άδεια χρήσης του στοιχείου. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Παρέχει άδεια χρήσης του στοιχείου. |

### Παραδείγματα

Δείχνει πώς να φορτώσετε μια άδεια χρήσης για το Aspose.Note από ένα αρχείο.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Δείχνει πώς να φορτώσετε μια άδεια για το Aspose.Note από μια ροή.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Δείχνει πώς να φορτώσετε μια άδεια χρήσης για το Aspose.Note από ενσωματωμένο πόρο αρχείου.

```csharp
// Δημιουργήστε την κλάση άδειας χρήσης
Aspose.Note.License license = new Aspose.Note.License();

// Περάστε μόνο το όνομα του αρχείου άδειας χρήσης που είναι ενσωματωμένο στη συγκρότηση
license.SetLicense("Aspose.Note.lic");
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


