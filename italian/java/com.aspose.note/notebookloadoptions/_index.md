---
title: "NotebookLoadOptions"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Opzioni utilizzate per caricare un taccuino."
type: docs
weight: 58
url: /it/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Opzioni utilizzate per caricare un taccuino.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Inizializza una nuova istanza della classe `NotebookLoadOptions`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Ottiene o imposta un valore che indica se i documenti figli devono essere caricati esplicitamente in seguito. |
| [getInstantLoading()](#getInstantLoading--) | Ottiene o imposta un valore che indica se i documenti figli devono essere caricati durante il caricamento del documento padre. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Ottiene o imposta un valore che indica se i documenti figli devono essere caricati esplicitamente in seguito. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Ottiene o imposta un valore che indica se i documenti figli devono essere caricati durante il caricamento del documento padre. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Inizializza una nuova istanza della classe `NotebookLoadOptions`.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Ottiene o imposta un valore che indica se i documenti figli devono essere caricati esplicitamente in seguito.

--------------------

Il valore predefinito è `false`, quindi i documenti figlio verranno caricati implicitamente. Il valore `true` indica che l'utente dovrebbe chiamare `Notebook.loadChildDocument` o per ogni nodo figlio del notebook dopo che il notebook stesso è stato caricato. Se il valore è `true`, l'opzione `NotebookLoadOptions.instantLoading` verrà ignorata. Se il notebook viene caricato da uno stream, il valore è sempre `true` nonostante sia stato impostato esplicitamente dall'utente a `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Ottiene o imposta un valore che indica se i documenti figli devono essere caricati durante il caricamento del documento padre.

--------------------

Il valore predefinito è `false`, quindi i documenti figlio verranno caricati \"pigramente\", cioè il loro caricamento dovrebbe essere posticipato fino a un accesso diretto al figlio specifico. Il valore `true` indica che il loro caricamento dovrebbe avvenire immediatamente.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Ottiene o imposta un valore che indica se i documenti figli devono essere caricati esplicitamente in seguito.

--------------------

Il valore predefinito è `false`, quindi i documenti figlio verranno caricati implicitamente. Il valore `true` indica che l'utente dovrebbe chiamare `Notebook.loadChildDocument` o per ogni nodo figlio del notebook dopo che il notebook stesso è stato caricato. Se il valore è `true`, l'opzione `NotebookLoadOptions.instantLoading` verrà ignorata. Se il notebook viene caricato da uno stream, il valore è sempre `true` nonostante sia stato impostato esplicitamente dall'utente a `false`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Ottiene o imposta un valore che indica se i documenti figli devono essere caricati durante il caricamento del documento padre.

--------------------

Il valore predefinito è `false`, quindi i documenti figlio verranno caricati \"pigramente\", cioè il loro caricamento dovrebbe essere posticipato fino a un accesso diretto al figlio specifico. Il valore `true` indica che il loro caricamento dovrebbe avvenire immediatamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

