---
title: "Notebook"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un cuaderno Aspose.Note."
type: docs
weight: 56
url: /es/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Representa un cuaderno Aspose.Note.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Notebook()](#Notebook--) | Inicializa una nueva instancia de la clase `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Inicializa una nueva instancia de la clase `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Inicializa una nueva instancia de la clase `Notebook`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Obtiene todos los nodos hijos por el tipo de nodo. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Agrega el nodo al final de la lista. |
| [getColor()](#getColor--) | Obtiene o establece el color. |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en el `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Obtiene o establece el nombre para mostrar. |
| [getFileFormat()](#getFileFormat--) | Obtiene el formato de archivo (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Obtiene el identificador único global del objeto. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Obtiene el nodo hijo del cuaderno mediante el índice proporcionado. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Obtiene o establece un valor que indica si el historial está habilitado. |
| [iterator()](#iterator--) | Devuelve un enumerador que itera a través de los nodos hijos del `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Agrega un nodo de documento hijo. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Agrega un nodo de documento hijo. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Agrega un nodo de documento hijo. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Agrega un nodo de documento hijo. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Agrega un nodo de cuaderno hijo. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Agrega un nodo de cuaderno hijo. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Elimina el nodo hijo. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Guarda el documento OneNote en un flujo. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Guarda el documento OneNote en un flujo usando las opciones de guardado especificadas. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Guarda el documento OneNote en un flujo en el formato especificado. |
| [save(String fileName)](#save-java.lang.String-) | Guarda el documento OneNote en un archivo. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Guarda el documento OneNote en un archivo usando las opciones de guardado especificadas. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Guarda el documento OneNote en un archivo en el formato especificado. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Obtiene o establece el color. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Obtiene o establece el nombre para mostrar. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Obtiene o establece un valor que indica si el historial está habilitado. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Inicializa una nueva instancia de la clase `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Inicializa una nueva instancia de la clase `Notebook`. Abre un cuaderno OneNote existente desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase `Notebook`. Abre un cuaderno de OneNote existente desde un archivo. Permite especificar opciones adicionales como una estrategia de carga de hijos ("lazy"/instant).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Las opciones de carga. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Obtiene todos los nodos hijos por el tipo de nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Una lista de nodos hijos.

`T1`: El tipo de elementos en la lista devuelta.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Agrega el nodo al final de la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | El nodo a agregar. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Obtiene o establece el color.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de elementos contenidos en el `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtiene o establece el nombre para mostrar.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Obtiene el formato de archivo (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Obtiene el identificador único global del objeto.

Valor: El GUID.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


Obtiene el nodo hijo del cuaderno mediante el índice proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | Índice al nodo hijo. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Obtiene o establece un valor que indica si el historial está habilitado.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Devuelve un enumerador que itera a través de los nodos hijos del `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Un `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Agrega un nodo de documento hijo. Abre un documento de OneNote existente desde un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Agrega un nodo de documento hijo. Abre un documento de OneNote existente desde un flujo. Permite especificar opciones de carga adicionales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Las opciones de carga. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Agrega un nodo de documento hijo. Abre un documento de OneNote existente desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Agrega un nodo de documento hijo. Abre un documento de OneNote existente desde un archivo. Permite especificar opciones de carga adicionales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Las opciones de carga. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Agrega un nodo de cuaderno hijo. Abre un cuaderno de OneNote existente desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Agrega un nodo de cuaderno hijo. Abre un cuaderno de OneNote existente desde un archivo. Permite especificar opciones de carga adicionales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Las opciones de carga. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Elimina el nodo hijo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | El nodo a eliminar. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Guarda el documento OneNote en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | El flujo. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Guarda el documento OneNote en un flujo usando las opciones de guardado especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | El flujo. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Especifica las opciones de cómo se guarda el documento. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Guarda el documento OneNote en un flujo en el formato especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | El flujo. |
| format | int | El formato en el que guardar el documento. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Guarda el documento OneNote en un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, el archivo existente se sobrescribe. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Guarda el documento OneNote en un archivo usando las opciones de guardado especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, el archivo existente se sobrescribe. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Especifica las opciones de cómo se guarda el documento en el archivo. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Guarda el documento OneNote en un archivo en el formato especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, el archivo existente se sobrescribe. |
| format | int | El formato en el que guardar el documento. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Obtiene o establece el color.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Obtiene o establece el nombre para mostrar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Obtiene o establece un valor que indica si el historial está habilitado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

