---
title: "NotebookLoadOptions"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Opciones usadas para cargar un cuaderno."
type: docs
weight: 58
url: /es/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Opciones usadas para cargar un cuaderno.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Inicializa una nueva instancia de la clase `NotebookLoadOptions`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Obtiene o establece un valor que indica si los documentos hijos deben cargarse explícitamente más tarde. |
| [getInstantLoading()](#getInstantLoading--) | Obtiene o establece un valor que indica si los documentos hijos deben cargarse mientras se carga el documento padre. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Obtiene o establece un valor que indica si los documentos hijos deben cargarse explícitamente más tarde. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Obtiene o establece un valor que indica si los documentos hijos deben cargarse mientras se carga el documento padre. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Inicializa una nueva instancia de la clase `NotebookLoadOptions`.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Obtiene o establece un valor que indica si los documentos hijos deben cargarse explícitamente más tarde.

--------------------

El valor predeterminado es `false`, por lo que los documentos hijos se cargarán implícitamente. El valor `true` indica que el usuario debe llamar a `Notebook.loadChildDocument` o a cada nodo hijo del cuaderno después de que el propio cuaderno se haya cargado. Si el valor es `true`, se ignorará la opción `NotebookLoadOptions.instantLoading`. Si el cuaderno se está cargando desde un flujo, el valor siempre es `true` a pesar de haber sido establecido explícitamente por el usuario a `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Obtiene o establece un valor que indica si los documentos hijos deben cargarse mientras se carga el documento padre.

--------------------

El valor predeterminado es `false`, por lo que los documentos hijos se cargarán "perezosamente", es decir, su carga debe posponerse hasta un acceso directo a un hijo específico. El valor `true` indica que su carga debe realizarse inmediatamente.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Obtiene o establece un valor que indica si los documentos hijos deben cargarse explícitamente más tarde.

--------------------

El valor predeterminado es `false`, por lo que los documentos hijos se cargarán implícitamente. El valor `true` indica que el usuario debe llamar a `Notebook.loadChildDocument` o a cada nodo hijo del cuaderno después de que el propio cuaderno se haya cargado. Si el valor es `true`, se ignorará la opción `NotebookLoadOptions.instantLoading`. Si el cuaderno se está cargando desde un flujo, el valor siempre es `true` a pesar de haber sido establecido explícitamente por el usuario a `false`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Obtiene o establece un valor que indica si los documentos hijos deben cargarse mientras se carga el documento padre.

--------------------

El valor predeterminado es `false`, por lo que los documentos hijos se cargarán "perezosamente", es decir, su carga debe posponerse hasta un acceso directo a un hijo específico. El valor `true` indica que su carga debe realizarse inmediatamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

