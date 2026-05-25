---
title: "ITag"
second_title: "Riferimento API di Aspose.Note per Java"
description: "L'interfaccia per i tag di ogni tipo."
type: docs
weight: 109
url: /it/java/com.aspose.note/itag/
---
```
public interface ITag
```

L'interfaccia per i tag di ogni tipo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Ottiene l'ora di completamento. |
| [getCreationTime()](#getCreationTime--) | Ottiene l'ora di creazione. |
| [getIcon()](#getIcon--) | Ottiene l'icona. |
| [getLabel()](#getLabel--) | Ottiene il testo dell'etichetta. |
| [getStatus()](#getStatus--) | Ottiene lo stato. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Imposta l'ora di creazione. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Ottiene l'ora di completamento.

Valore: Il `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Ottiene l'ora di creazione.

Valore: Il java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Ottiene l'icona.

Valore: Il [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Ottiene il testo dell'etichetta.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Ottiene lo stato.

Valore: Il [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Imposta l'ora di creazione.

Valore: Il java.util.Date.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

