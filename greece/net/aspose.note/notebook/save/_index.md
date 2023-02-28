---
title: Notebook.Save
second_title: Aspose.Note for .NET API Reference
description: Notebook μέθοδος. Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο.
type: docs
weight: 150
url: /el/net/aspose.note/notebook/save/
---
## Save(string) {#save_3}

Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο.

```csharp
public void Save(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη ένα αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο αντικαθίσταται. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Αποθηκεύει το έγγραφο του OneNote σε μια ροή.

```csharp
public void Save(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο στην καθορισμένη μορφή.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη ένα αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο αντικαθίσταται. |
| format | SaveFormat | Η μορφή με την οποία αποθηκεύεται το έγγραφο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Αποθηκεύει το έγγραφο του OneNote σε μια ροή με την καθορισμένη μορφή.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| format | SaveFormat | Η μορφή με την οποία αποθηκεύεται το έγγραφο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(string, NotebookSaveOptions) {#save_5}

Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void Save(string fileName, NotebookSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη ένα αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο αντικαθίσταται. |
| options | NotebookSaveOptions | Καθορίζει τις επιλογές για τον τρόπο αποθήκευσης του εγγράφου στο αρχείο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(Stream, NotebookSaveOptions) {#save_2}

Αποθηκεύει το έγγραφο του OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void Save(Stream stream, NotebookSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| options | NotebookSaveOptions | Καθορίζει τις επιλογές για τον τρόπο αποθήκευσης του εγγράφου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)


