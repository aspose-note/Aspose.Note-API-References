---
title: "CheckBox"
second_title: "Referencia de API de Aspose.Note para Java"
description: "La clase base para etiquetas que pueden alternar su estado entre completo e incompleto."
type: docs
weight: 13
url: /es/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

La clase base para etiquetas que pueden alternar su estado entre completo e incompleto.
## Métodos

| Método | Descripción |
| --- | --- |
| [getChecked()](#getChecked--) | Obtiene un valor que indica si el CheckBox está en estado marcado. |
| [getCompletedTime()](#getCompletedTime--) | Obtiene o establece la hora de finalización. |
| [getCreationTime()](#getCreationTime--) | Obtiene o establece la hora de creación. |
| [getIcon()](#getIcon--) | Obtiene o establece el ícono. |
| [getStatus()](#getStatus--) | Obtiene o establece el estado. |
| [setCompleted()](#setCompleted--) | Establece la etiqueta al estado completado usando la hora actual como hora de finalización. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Establece la etiqueta al estado completado. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Obtiene o establece la hora de creación. |
| [setOpen()](#setOpen--) | Establece la etiqueta en estado abierto. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Obtiene un valor que indica si el CheckBox está en estado marcado.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Obtiene o establece la hora de finalización.

Valor: El `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtiene o establece la hora de creación.

Valor: El java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Obtiene o establece el ícono.

Valor: El [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Obtiene o establece el estado.

Valor: El [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Establece la etiqueta al estado completado usando la hora actual como hora de finalización.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Establece la etiqueta al estado completado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| completedTime | java.util.Date | La hora de finalización. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Obtiene o establece la hora de creación.

Valor: El java.util.Date.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Establece la etiqueta en estado abierto.

