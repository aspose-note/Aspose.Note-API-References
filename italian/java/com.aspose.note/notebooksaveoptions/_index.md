---
title: "NotebookSaveOptions"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Una classe base astratta che rappresenta le opzioni di salvataggio del taccuino per un formato specifico."
type: docs
weight: 61
url: /it/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Una classe base astratta che rappresenta le opzioni di salvataggio del taccuino per un formato specifico.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Ottiene o imposta un valore che indica se i documenti figli devono essere salvati esplicitamente. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Ottiene le opzioni di salvataggio per tutti i documenti figli del notebook. |
| [getFlatten()](#getFlatten--) | Ottiene o imposta un valore che indica se la gerarchia dei figli del notebook viene salvata appiattita. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato in cui il notebook viene salvato. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Ottiene o imposta un valore che indica se i documenti figli devono essere salvati esplicitamente. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Ottiene o imposta un valore che indica se la gerarchia dei figli del notebook viene salvata appiattita. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Ottiene o imposta un valore che indica se i documenti figli devono essere salvati esplicitamente.

--------------------

Il valore predefinito è `false`, quindi i documenti figlio verranno salvati implicitamente. Il valore `true` indica che l'utente deve salvare esplicitamente ogni nodo figlio del notebook. Se il notebook viene salvato su stream, il valore è sempre `true` nonostante sia stato impostato esplicitamente dall'utente a `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Ottiene le opzioni di salvataggio per tutti i documenti figli del notebook.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Ottiene o imposta un valore che indica se la gerarchia dei figli del notebook viene salvata appiattita.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Ottiene il formato in cui il notebook viene salvato.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Ottiene o imposta un valore che indica se i documenti figli devono essere salvati esplicitamente.

--------------------

Il valore predefinito è `false`, quindi i documenti figlio verranno salvati implicitamente. Il valore `true` indica che l'utente deve salvare esplicitamente ogni nodo figlio del notebook. Se il notebook viene salvato su stream, il valore è sempre `true` nonostante sia stato impostato esplicitamente dall'utente a `false`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Ottiene o imposta un valore che indica se la gerarchia dei figli del notebook viene salvata appiattita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

