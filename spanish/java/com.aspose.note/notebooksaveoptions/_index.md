---
title: "NotebookSaveOptions"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular."
type: docs
weight: 61
url: /es/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular.
## Métodos

| Método | Descripción |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Obtiene o establece un valor que indica si los documentos hijos deben guardarse explícitamente. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Obtiene las opciones de guardado para todos los documentos hijos del cuaderno. |
| [getFlatten()](#getFlatten--) | Obtiene o establece un valor que indica si la jerarquía de los hijos del cuaderno se guarda aplanada. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato en el que se guarda el cuaderno. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Obtiene o establece un valor que indica si los documentos hijos deben guardarse explícitamente. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Obtiene o establece un valor que indica si la jerarquía de los hijos del cuaderno se guarda aplanada. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Obtiene o establece un valor que indica si los documentos hijos deben guardarse explícitamente.

--------------------

El valor predeterminado es `false`, por lo que los documentos secundarios se guardarán implícitamente. El valor `true` indica que el usuario debe guardar cada nodo secundario del cuaderno explícitamente. Si el cuaderno se guarda en un flujo, el valor siempre es `true` a pesar de que el usuario lo haya establecido explícitamente en `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Obtiene las opciones de guardado para todos los documentos hijos del cuaderno.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Obtiene o establece un valor que indica si la jerarquía de los hijos del cuaderno se guarda aplanada.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Obtiene el formato en el que se guarda el cuaderno.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Obtiene o establece un valor que indica si los documentos hijos deben guardarse explícitamente.

--------------------

El valor predeterminado es `false`, por lo que los documentos secundarios se guardarán implícitamente. El valor `true` indica que el usuario debe guardar cada nodo secundario del cuaderno explícitamente. Si el cuaderno se guarda en un flujo, el valor siempre es `true` a pesar de que el usuario lo haya establecido explícitamente en `false`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Obtiene o establece un valor que indica si la jerarquía de los hijos del cuaderno se guarda aplanada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

