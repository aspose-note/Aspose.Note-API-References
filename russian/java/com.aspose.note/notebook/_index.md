---
title: "Блокнот"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет блокнот Aspose.Note."
type: docs
weight: 56
url: /ru/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Представляет блокнот Aspose.Note.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Notebook()](#Notebook--) | Инициализирует новый экземпляр класса `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Инициализирует новый экземпляр класса `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Инициализирует новый экземпляр класса `Notebook`. |
## Методы

| Метод | Описание |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Получить все дочерние узлы по типу узла. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Добавляет узел в конец списка. |
| [getColor()](#getColor--) | Получает или задаёт цвет. |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Получает или задаёт отображаемое имя. |
| [getFileFormat()](#getFileFormat--) | Получает формат файла (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Получает глобальный уникальный идентификатор объекта. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Получает дочерний узел блокнота по заданному индексу. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Получает или задаёт значение, указывающее, включена ли история. |
| [iterator()](#iterator--) | Возвращает перечислитель, который перебирает дочерние узлы `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Добавляет дочерний узел документа. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Добавляет дочерний узел документа. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Добавляет дочерний узел документа. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Добавляет дочерний узел документа. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Добавляет дочерний узел блокнота. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Добавляет дочерний узел блокнота. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Удаляет дочерний узел. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Сохраняет документ OneNote в поток. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Сохраняет документ OneNote в поток, используя указанные параметры сохранения. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Сохраняет документ OneNote в поток в указанном формате. |
| [save(String fileName)](#save-java.lang.String-) | Сохраняет документ OneNote в файл. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Сохраняет документ OneNote в файл, используя указанные параметры сохранения. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Сохраняет документ OneNote в файл в указанном формате. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Получает или задаёт цвет. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Получает или задаёт отображаемое имя. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Получает или задаёт значение, указывающее, включена ли история. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Инициализирует новый экземпляр класса `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Инициализирует новый экземпляр класса `Notebook`. Открывает существующий блокнот OneNote из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса `Notebook`. Открывает существующий блокнот OneNote из файла. Позволяет указать дополнительные параметры, такие как стратегия загрузки дочерних элементов ("lazy"/instant).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Параметры загрузки. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Получить все дочерние узлы по типу узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Список дочерних узлов.

`T1`: Тип элементов в возвращаемом списке.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Добавляет узел в конец списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Узел для добавления. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Получает или задаёт цвет.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, содержащихся в `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Получает или задаёт отображаемое имя.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Получает формат файла (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Получает глобальный уникальный идентификатор объекта.

Значение: GUID.

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


Получает дочерний узел блокнота по заданному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Индекс дочернего узла. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Получает или задаёт значение, указывающее, включена ли история.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Возвращает перечислитель, который перебирает дочерние узлы `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Добавляет дочерний узел документа. Открывает существующий документ OneNote из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Добавляет дочерний узел документа. Открывает существующий документ OneNote из потока. Позволяет указать дополнительные параметры загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Параметры загрузки. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Добавляет дочерний узел документа. Открывает существующий документ OneNote из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Добавляет дочерний узел документа. Открывает существующий документ OneNote из файла. Позволяет указать дополнительные параметры загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Параметры загрузки. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Добавляет дочерний узел блокнота. Открывает существующий блокнот OneNote из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Добавляет дочерний узел блокнота. Открывает существующий блокнот OneNote из файла. Позволяет указать дополнительные параметры загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Параметры загрузки. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Удаляет дочерний узел.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Узел для удаления. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Сохраняет документ OneNote в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | Поток. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Сохраняет документ OneNote в поток, используя указанные параметры сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | Поток. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Указывает параметры сохранения документа. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Сохраняет документ OneNote в поток в указанном формате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | Поток. |
| format | int | Формат, в котором сохраняется документ. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Сохраняет документ OneNote в файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл будет перезаписан. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Сохраняет документ OneNote в файл, используя указанные параметры сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл будет перезаписан. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Указывает параметры, как документ сохраняется в файл. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Сохраняет документ OneNote в файл в указанном формате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл будет перезаписан. |
| format | int | Формат, в котором сохраняется документ. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Получает или задаёт цвет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Получает или задаёт отображаемое имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Получает или задаёт значение, указывающее, включена ли история.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

