---
title: "ITag"
second_title: "Referencia de API de Aspose.Note para Java"
description: "La interfaz para etiquetas de todo tipo."
type: docs
weight: 109
url: /es/java/com.aspose.note/itag/
---
```
public interface ITag
```

La interfaz para etiquetas de todo tipo.
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Obtiene la hora de finalización. |
| [getCreationTime()](#getCreationTime--) | Obtiene la hora de creación. |
| [getIcon()](#getIcon--) | Obtiene el ícono. |
| [getLabel()](#getLabel--) | Obtiene el texto de la etiqueta. |
| [getStatus()](#getStatus--) | Obtiene el estado. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Establece la hora de creación. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Obtiene la hora de finalización.

Valor: El `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Obtiene la hora de creación.

Valor: El java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Obtiene el ícono.

Valor: El [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Obtiene el texto de la etiqueta.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Obtiene el estado.

Valor: El [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Establece la hora de creación.

Valor: El java.util.Date.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

