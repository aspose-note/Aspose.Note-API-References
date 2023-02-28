---
title: Document.Document
second_title: Aspose.Note for .NET API Reference
description: Document κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουDocument class. Δημιουργεί ένα κενό έγγραφο OneNote.
type: docs
weight: 10
url: /el/net/aspose.note/document/document/
---
## Document() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Document`](../) class. Δημιουργεί ένα κενό έγγραφο OneNote.

```csharp
public Document()
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία του[`Document`](../) class. Ανοίγει ένα υπάρχον έγγραφο OneNote από ένα αρχείο.

```csharp
public Document(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Η μορφή του εγγράφου δεν αναγνωρίζεται ή δεν υποστηρίζεται. |
| [FileCorruptedException](../../filecorruptedexception/) | Το έγγραφο φαίνεται να είναι κατεστραμμένο και δεν μπορεί να φορτωθεί. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Το έγγραφο είναι κρυπτογραφημένο και απαιτεί κωδικό πρόσβασης για να ανοίξει, αλλά εσείς παρείχατε εσφαλμένο κωδικό πρόσβασης. |
| InvalidOperationException | Υπάρχει πρόβλημα με το έγγραφο και θα πρέπει να αναφερθεί στους προγραμματιστές του Aspose.Note. |
| IOException | Υπάρχει εξαίρεση εισόδου/εξόδου. |

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία του[`Document`](../)class. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών, όπως έναν κωδικό πρόσβασης κρυπτογράφησης.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |
| loadOptions | LoadOptions | Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός εγγράφου. Μπορεί να είναι null. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Η μορφή του εγγράφου δεν αναγνωρίζεται ή δεν υποστηρίζεται. |
| [FileCorruptedException](../../filecorruptedexception/) | Το έγγραφο φαίνεται να είναι κατεστραμμένο και δεν μπορεί να φορτωθεί. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Το έγγραφο είναι κρυπτογραφημένο και απαιτεί κωδικό πρόσβασης για να ανοίξει, αλλά εσείς παρείχατε εσφαλμένο κωδικό πρόσβασης. |
| InvalidOperationException | Υπάρχει πρόβλημα με το έγγραφο και θα πρέπει να αναφερθεί στους προγραμματιστές του Aspose.Note. |
| IOException | Υπάρχει εξαίρεση εισόδου/εξόδου. |

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Document`](../) class. Ανοίγει ένα υπάρχον έγγραφο OneNote από μια ροή.

```csharp
public Document(Stream inStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inStream | Stream | Η ροή. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Η μορφή του εγγράφου δεν αναγνωρίζεται ή δεν υποστηρίζεται. |
| [FileCorruptedException](../../filecorruptedexception/) | Το έγγραφο φαίνεται να είναι κατεστραμμένο και δεν μπορεί να φορτωθεί. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Το έγγραφο είναι κρυπτογραφημένο και απαιτεί κωδικό πρόσβασης για να ανοίξει, αλλά εσείς παρείχατε εσφαλμένο κωδικό πρόσβασης. |
| InvalidOperationException | Υπάρχει πρόβλημα με το έγγραφο και θα πρέπει να αναφερθεί στους προγραμματιστές του Aspose.Note. |
| IOException | Υπάρχει εξαίρεση εισόδου/εξόδου. |
| ArgumentException | Η ροή δεν υποστηρίζει ανάγνωση, είναι μηδενική ή είναι ήδη κλειστή. |

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`Document`](../) class. Ανοίγει ένα υπάρχον έγγραφο OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών, όπως έναν κωδικό πρόσβασης κρυπτογράφησης.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inStream | Stream | Η ροή. |
| loadOptions | LoadOptions | Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός εγγράφου. Μπορεί να είναι null. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Η μορφή του εγγράφου δεν αναγνωρίζεται ή δεν υποστηρίζεται. |
| [FileCorruptedException](../../filecorruptedexception/) | Το έγγραφο φαίνεται να είναι κατεστραμμένο και δεν μπορεί να φορτωθεί. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Το έγγραφο είναι κρυπτογραφημένο και απαιτεί κωδικό πρόσβασης για να ανοίξει, αλλά εσείς παρείχατε εσφαλμένο κωδικό πρόσβασης. |
| InvalidOperationException | Υπάρχει πρόβλημα με το έγγραφο και θα πρέπει να αναφερθεί στους προγραμματιστές του Aspose.Note. |
| IOException | Υπάρχει εξαίρεση εισόδου/εξόδου. |
| ArgumentException | Η ροή δεν υποστηρίζει ανάγνωση, είναι μηδενική ή είναι ήδη κλειστή. |

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


