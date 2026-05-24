---
title: "Document"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل مستند Aspose.Note."
type: docs
weight: 20
url: /ar/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

يمثل مستند Aspose.Note.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Document()](#Document--) | يُنشئ مثلاً جديدًا من الفئة `Document` class. |
| [Document(String filePath)](#Document-java.lang.String-) | يُنشئ مثلاً جديدًا من الفئة `Document` class. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | يُنشئ مثلاً جديدًا من الفئة `Document` class. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | يُنشئ مثلاً جديدًا من الفئة `Document` class. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | يُنشئ مثلاً جديدًا من الفئة `Document` class. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [detectLayoutChanges()](#detectLayoutChanges--) | يكشف جميع التغييرات التي طرأت على تخطيط المستند منذ الاستدعاء السابق لـ `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | يحصل على قيمة تشير إلى ما إذا كان Aspose.Note يقوم بالكشف عن تغييرات التخطيط تلقائيًا. |
| [getColor()](#getColor--) | يحصل على اللون. |
| [getCreationTime()](#getCreationTime--) | يحصل على وقت الإنشاء. |
| [getDisplayName()](#getDisplayName--) | يحصل على اسم العرض. |
| [getFileFormat()](#getFileFormat--) | يحصل على تنسيق الملف (OneNote 2010، OneNote Online). |
| [getGuid()](#getGuid--) | يحصل على المعرف الفريد عالميًا للكائن. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | يحصل على `PageHistory` الذي يحتوي على السجل الكامل لكل صفحة معروضة في مستند (الأقدم في الفهرس 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | يتحقق مما إذا كان المستند من تدفق مشفرًا. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | يتحقق مما إذا كان المستند من تدفق مشفرًا. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | يتحقق مما إذا كان المستند من تدفق مشفرًا. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | يتحقق مما إذا كان المستند من ملف مشفرًا. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | يتحقق مما إذا كان المستند من ملف مشفرًا. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | يتحقق مما إذا كان المستند من ملف مشفرًا. |
| [print()](#print--) | يطبع المستند باستخدام الطابعة الافتراضية. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | يطبع المستند باستخدام الطابعة الافتراضية. |
| [print(String printerName)](#print-java.lang.String-) | يطبع المستند باستخدام الطابعة الافتراضية. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | يطبع المستند باستخدام الطابعة الافتراضية. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | يحفظ مستند OneNote إلى تدفق. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد. |
| [save(String fileName)](#save-java.lang.String-) | يحفظ مستند OneNote إلى ملف. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | يحفظ مستند OneNote إلى ملف بالتنسيق المحدد. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | يضبط قيمة تشير إلى ما إذا كان Aspose.Note يقوم بالكشف عن تغييرات التخطيط تلقائيًا. |
| [setColor(Color value)](#setColor-java.awt.Color-) | يضبط اللون. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | يضبط وقت الإنشاء. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | يضبط اسم العرض. |
### Document() {#Document--}
```
public Document()
```


يُنشئ مثيلاً جديدًا لفئة `Document`. ينشئ مستند OneNote فارغًا.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


يُنشئ مثيلاً جديدًا لفئة `Document`. يفتح مستند OneNote موجود من ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


يُنشئ مثيلاً جديدًا لفئة `Document`. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | الخيارات المستخدمة لتحميل مستند. يمكن أن تكون فارغة. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


يُنشئ مثيلاً جديدًا لفئة `Document`. يفتح مستند OneNote موجود من تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inStream | java.io.InputStream | التدفق. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


يُنشئ مثيلاً جديدًا لفئة `Document`. يفتح مستند OneNote موجود من تدفق. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inStream | java.io.InputStream | التدفق. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | الخيارات المستخدمة لتحميل مستند. يمكن أن تكون فارغة. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


يكشف عن جميع التغييرات التي تم إجراؤها على تخطيط المستند منذ استدعاء `DetectLayoutChanges` السابق. في حالة ضبط `AutomaticLayoutChangesDetectionEnabled` على true، يتم استخدامها تلقائيًا في بداية تصدير المستند.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


يحصل على قيمة تشير إلى ما إذا كان Aspose.Note يقوم بالكشف عن تغييرات التخطيط تلقائيًا. القيمة الافتراضية هي `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


يحصل على اللون.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


يحصل على وقت الإنشاء.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


يحصل على اسم العرض.

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

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


يحصل على `PageHistory` الذي يحتوي على السجل الكامل لكل صفحة معروضة في مستند (الأقدم في الفهرس 0). يمكن الوصول إلى نسخة الصفحة الحالية كـ `PageHistory.current` وتكون منفصلة عن مجموعة الإصدارات التاريخية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | النسخة الحالية لصفحة. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذلك قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | التدفق. |
| document | [Document\[\]](../../com.aspose.note/document) | المستند المحمَّل. |

**Returns:**
منطقي - يرجع true إذا كان المستند مشفرًا وإلا false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذلك قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | التدفق. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | خيارات التحميل. |
| document | [Document\[\]](../../com.aspose.note/document) | المستند المحمَّل. |

**Returns:**
منطقي - يرجع true إذا كان المستند مشفرًا وإلا false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذلك قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | التدفق. |
| password | java.lang.String | كلمة المرور لفك تشفير مستند. |
| document | [Document\[\]](../../com.aspose.note/document) | المستند المحمَّل. |

**Returns:**
منطقي - يرجع true إذا كان المستند مشفرًا وإلا false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذلك قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| document | [Document\[\]](../../com.aspose.note/document) | المستند المحمَّل. |

**Returns:**
منطقي - يرجع true إذا كان المستند مشفرًا وإلا false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذلك قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | خيارات التحميل. |
| document | [Document\[\]](../../com.aspose.note/document) | المستند المحمَّل. |

**Returns:**
منطقي - يرجع true إذا كان المستند مشفرًا وإلا false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذلك قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| password | java.lang.String | كلمة المرور لفك تشفير مستند. |
| document | [Document\[\]](../../com.aspose.note/document) | المستند المحمَّل. |

**Returns:**
منطقي - يرجع true إذا كان المستند مشفرًا وإلا false.
### print() {#print--}
```
public void print()
```


يطبع المستند باستخدام الطابعة الافتراضية.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


يطبع المستند باستخدام الطابعة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | الخيارات المستخدمة لطباعة مستند. يمكن أن تكون فارغة. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


يطبع المستند باستخدام الطابعة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


يطبع المستند باستخدام الطابعة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


يحفظ مستند OneNote إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.OutputStream | دفق System.iO حيث سيتم حفظ المستند. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.OutputStream | دفق System.iO حيث سيتم حفظ المستند. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | يحدد الخيارات لكيفية حفظ المستند في الدفق. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.OutputStream | دفق System.iO حيث سيتم حفظ المستند. |
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

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | الاسم الكامل للملف. إذا كان هناك ملف بالاسم الكامل المحدد موجودًا بالفعل، سيتم استبدال الملف الموجود. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | يحدد الخيارات التي يتم حفظ المستند بها في الملف. |

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

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان Aspose.Note يقوم بالكشف عن تغييرات التخطيط تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | قيمة جديدة. يمكن أن تكون فارغة. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


يضبط اللون.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color | قيمة اللون. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


يضبط وقت الإنشاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


يضبط اسم العرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة DateTime. |

