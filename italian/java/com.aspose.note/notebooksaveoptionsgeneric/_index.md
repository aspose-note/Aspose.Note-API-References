---
title: "NotebookSaveOptionsGeneric"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Una classe base astratta che rappresenta le opzioni di salvataggio del taccuino per un formato specifico e fornisce opzioni di salvataggio comuni per tutti i nodi figlio del documento."
type: docs
weight: 62
url: /it/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Una classe base astratta che rappresenta le opzioni di salvataggio del taccuino per un formato specifico e fornisce opzioni di salvataggio comuni per tutti i nodi figlio del documento.

`TDocumentSaveOptions`: Le opzioni di salvataggio per tutti i documenti figlio del notebook.

TDocumentSaveOptions :
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Ottiene o imposta le opzioni di salvataggio per tutti i documenti figlio del notebook. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Ottiene le opzioni di salvataggio per tutti i documenti figli del notebook. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato in cui il notebook viene salvato. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Ottiene o imposta le opzioni di salvataggio per tutti i documenti figlio del notebook.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Ottiene le opzioni di salvataggio per tutti i documenti figli del notebook.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene il formato in cui il notebook viene salvato.

**Returns:**
int
