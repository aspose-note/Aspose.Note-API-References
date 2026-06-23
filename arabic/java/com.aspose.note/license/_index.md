---
title: "License"
second_title: "مرجع Aspose.Note لـ Java API"
description: "يوفر طرقًا لترخيص المكوّن."
type: docs
weight: 44
url: /ar/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

يوفر طرقًا لترخيص المكوّن.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [License()](#License--) | ينشئ مثيلًا جديدًا لهذه الفئة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | يعيد تعيين سياق الرخصة للخيط الحالي. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | يُرخص المكوّن. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | يُرخص المكوّن. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | يُرخص المكوّن. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | يضبط سياق الرخصة للخيط الحالي. |
### License() {#License--}
```
public License()
```


ينشئ مثيلًا جديدًا لهذه الفئة.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


يعيد تعيين سياق الرخصة للخيط الحالي.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


يُرخص المكوّن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| licenseFile | java.io.File | ملف الرخصة`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


يُرخص المكوّن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | دفق | java.io.InputStream | دفق يحتوي على الرخصة. |

--------------------

`

استخدم هذه الطريقة لتحميل ترخيص من تدفق.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


يُرخص المكوّن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | licenseName | java.lang.String | يمكن أن يكون اسم ملف كامل أو قصير` أو اسم مورد مضمّن`. استخدم سلسلة فارغة للتبديل إلى وضع التقييم. |

--------------------

`

يحاول العثور على الترخيص في المواقع التالية:

` `

1. مسار صريح.

` `

2. المجلد الذي يحتوي على تجميع مكوّن Aspose.

3. المجلد الذي يحتوي على تجميع استدعاء العميل.

4. المجلد الذي يحتوي على تجميع الدخول (بدء التشغيل).

5. مورد مضمّن في تجميع استدعاء العميل.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. مسار صريح.

2. مورد مضمّن في تجميع استدعاء العميل.

` `

2. المجلد الذي يحتوي على ملف JAR لمكوّن Aspose.

3. المجلد الذي يحتوي على ملف JAR لاستدعاء العميل.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


يضبط سياق الرخصة للخيط الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | دفق يحتوي على الرخصة. |

