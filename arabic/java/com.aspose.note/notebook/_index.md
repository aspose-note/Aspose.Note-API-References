---
title: "دفتر الملاحظات"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل دفتر ملاحظات **Aspose.Note**."
type: docs
weight: 56
url: /ar/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

يمثل دفتر ملاحظات **Aspose.Note**.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Notebook()](#Notebook--) | يُهيئ نسخة جديدة من الفئة `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | يُهيئ نسخة جديدة من الفئة `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | يُهيئ نسخة جديدة من الفئة `Notebook`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | احصل على جميع العقد الفرعية وفقًا لنوع العقدة. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | يضيف العقدة إلى نهاية القائمة. |
| [getColor()](#getColor--) | يحصل على اللون أو يضبطه. |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في `Notebook`. |
| [getDisplayName()](#getDisplayName--) | يحصل على اسم العرض أو يضبطه. |
| [getFileFormat()](#getFileFormat--) | يحصل على تنسيق الملف (OneNote 2010، OneNote Online). |
| [getGuid()](#getGuid--) | يحصل على المعرف الفريد عالميًا للكائن. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | يحصل على عقدة فرعية للدفتر وفقًا للفهرس المعطى. |
| [isHistoryEnabled()](#isHistoryEnabled--) | يحصل على قيمة أو يضبطها تشير إلى ما إذا كان السجل مفعلاً. |
| [iterator()](#iterator--) | يرجع عدّادًا يتنقل عبر العقد الفرعية لـ `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | يضيف عقدة مستند فرعية. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | يضيف عقدة مستند فرعية. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | يضيف عقدة مستند فرعية. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | يضيف عقدة مستند فرعية. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | يضيف عقدة دفتر ملاحظات فرعية. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | يضيف عقدة دفتر ملاحظات فرعية. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | يزيل العقدة الفرعية. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | يحفظ مستند OneNote إلى تدفق. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد. |
| [save(String fileName)](#save-java.lang.String-) | يحفظ مستند OneNote إلى ملف. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | يحفظ مستند OneNote إلى ملف بالتنسيق المحدد. |
| [setColor(Color value)](#setColor-java.awt.Color-) | يحصل على اللون أو يضبطه. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | يحصل على اسم العرض أو يضبطه. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | يحصل على قيمة أو يضبطها تشير إلى ما إذا كان السجل مفعلاً. |
### Notebook() {#Notebook--}
```
public Notebook()
```


يُهيئ نسخة جديدة من الفئة `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


يُهيئ نسخة جديدة من الفئة `Notebook`. يفتح دفتر ملاحظات OneNote موجود من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


يقوم بإنشاء نسخة جديدة من الفئة `Notebook`. يفتح دفتر OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل استراتيجية تحميل الأطفال (\"lazy\"/instant).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | خيارات التحميل. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


احصل على جميع العقد الفرعية وفقًا لنوع العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - قائمة بالعقد الفرعية.

`T1`: نوع العناصر في القائمة المعادة.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


يضيف العقدة إلى نهاية القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | العقدة المراد إضافتها. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


يحصل على اللون أو يضبطه.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


يحصل على اسم العرض أو يضبطه.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


يحصل على تنسيق الملف (OneNote 2010، OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


يحصل على المعرف الفريد عالميًا للكائن.

القيمة: GUID.

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


يحصل على عقدة فرعية للدفتر وفقًا للفهرس المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | فهرس إلى العقدة الفرعية. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


يحصل على قيمة أو يضبطها تشير إلى ما إذا كان السجل مفعلاً.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


يرجع عدّادًا يتنقل عبر العقد الفرعية لـ `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


يضيف عقدة مستند فرعية. يفتح مستند OneNote موجود من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | التدفق. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


يضيف عقدة مستند فرعية. يفتح مستند OneNote موجود من تدفق. يسمح بتحديد خيارات تحميل إضافية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | التدفق. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | خيارات التحميل. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


يضيف عقدة مستند فرعية. يفتح مستند OneNote موجود من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


يضيف عقدة مستند فرعية. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات تحميل إضافية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | خيارات التحميل. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


يضيف عقدة دفتر ملاحظات فرعية. يفتح دفتر OneNote موجود من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


يضيف عقدة دفتر ملاحظات فرعية. يفتح دفتر OneNote موجود من ملف. يسمح بتحديد خيارات تحميل إضافية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | خيارات التحميل. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


يزيل العقدة الفرعية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | العقدة المراد إزالتها. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


يحفظ مستند OneNote إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.OutputStream | التدفق. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.OutputStream | التدفق. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | يحدد الخيارات لكيفية حفظ المستند. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.OutputStream | التدفق. |
| format | int | الصيغة التي سيتم حفظ المستند بها. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


يحفظ مستند OneNote إلى ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، سيتم استبدال الملف الموجود. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، سيتم استبدال الملف الموجود. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | يحدد الخيارات التي يتم حفظ المستند بها في الملف. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


يحفظ مستند OneNote إلى ملف بالتنسيق المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، سيتم استبدال الملف الموجود. |
| format | int | الصيغة التي سيتم حفظ المستند بها. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


يحصل على اللون أو يضبطه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


يحصل على اسم العرض أو يضبطه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


يحصل على قيمة أو يضبطها تشير إلى ما إذا كان السجل مفعلاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

