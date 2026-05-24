---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Μια αφηρημένη βασική κλάση που αντιπροσωπεύει τις επιλογές αποθήκευσης του σημειωματάριου για μια συγκεκριμένη μορφή και παρέχει κοινές επιλογές αποθήκευσης για όλους τους θυγατρικούς κόμβους του εγγράφου."
type: docs
weight: 62
url: /el/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Μια αφηρημένη βασική κλάση που αντιπροσωπεύει τις επιλογές αποθήκευσης του σημειωματάριου για μια συγκεκριμένη μορφή και παρέχει κοινές επιλογές αποθήκευσης για όλους τους θυγατρικούς κόμβους του εγγράφου.

`TDocumentSaveOptions`: Οι επιλογές αποθήκευσης για όλα τα παιδικά έγγραφα του σημειωματάριου.

TDocumentSaveOptions :
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Λαμβάνει ή ορίζει τις επιλογές αποθήκευσης για όλα τα παιδικά έγγραφα του σημειωματάριου. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Λαμβάνει τις επιλογές αποθήκευσης για όλα τα έγγραφα παιδιών του σημειωματάριου. |
| [getSaveFormat()](#getSaveFormat--) | Λαμβάνει τη μορφή με την οποία αποθηκεύεται το σημειωματάριο. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Λαμβάνει ή ορίζει τις επιλογές αποθήκευσης για όλα τα παιδικά έγγραφα του σημειωματάριου.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Λαμβάνει τις επιλογές αποθήκευσης για όλα τα έγγραφα παιδιών του σημειωματάριου.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Λαμβάνει τη μορφή με την οποία αποθηκεύεται το σημειωματάριο.

**Returns:**
int
