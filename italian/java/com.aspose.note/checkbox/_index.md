---
title: "CheckBox"
second_title: "Riferimento API di Aspose.Note per Java"
description: "La classe base per i tag che possono alternare il loro stato tra completo e incompleto."
type: docs
weight: 13
url: /it/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

La classe base per i tag che possono alternare il loro stato tra completo e incompleto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getChecked()](#getChecked--) | Ottiene un valore che indica se la CheckBox è nello stato selezionato. |
| [getCompletedTime()](#getCompletedTime--) | Ottiene o imposta l'ora di completamento. |
| [getCreationTime()](#getCreationTime--) | Ottiene o imposta l'ora di creazione. |
| [getIcon()](#getIcon--) | Ottiene o imposta l'icona. |
| [getStatus()](#getStatus--) | Ottiene o imposta lo stato. |
| [setCompleted()](#setCompleted--) | Imposta il tag allo stato completato usando l'ora corrente come ora di completamento. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Imposta il tag allo stato completato. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Ottiene o imposta l'ora di creazione. |
| [setOpen()](#setOpen--) | Imposta il tag in stato aperto. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Ottiene un valore che indica se la CheckBox è nello stato selezionato.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Ottiene o imposta l'ora di completamento.

Valore: Il `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Ottiene o imposta l'ora di creazione.

Valore: Il java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Ottiene o imposta l'icona.

Valore: Il [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Ottiene o imposta lo stato.

Valore: Il [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Imposta il tag allo stato completato usando l'ora corrente come ora di completamento.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Imposta il tag allo stato completato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| completedTime | java.util.Date | Il tempo di completamento. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Ottiene o imposta l'ora di creazione.

Valore: Il java.util.Date.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Imposta il tag in stato aperto.

