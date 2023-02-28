---
title: Notebook.LoadChildDocument
second_title: Aspose.Note for .NET API Reference
description: Notebook μέθοδος. Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο.
type: docs
weight: 120
url: /el/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο.

```csharp
public void LoadChildDocument(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |

### Παραδείγματα

Δείχνει πώς να φορτώσετε το σημειωματάριο από μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Δείτε επίσης

* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Η διαδρομή του αρχείου. |
| loadOptions | LoadOptions | Οι επιλογές φόρτωσης. |

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από μια ροή.

```csharp
public void LoadChildDocument(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |

### Παραδείγματα

Δείχνει πώς να φορτώσετε το σημειωματάριο από μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Δείτε επίσης

* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| loadOptions | LoadOptions | Οι επιλογές φόρτωσης. |

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)


