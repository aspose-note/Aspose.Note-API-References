---
title: "FontsSubsystem"
second_title: "مرجع Aspose.Note for Java API"
description: "الفئة الأساسية التي تنفذ واجهة com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /ar/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

الفئة الأساسية التي تنفّذ واجهة com.aspose.note.IFontsSubsystem. توفر وظائف الخط الافتراضي واستبدالات الخط. قم بتجاوز الدالة المحمية com.aspose.note.FontsSubsystem.fetchFontFamily في فئة مشتقة لتنفيذ المنطق لاسترجاع كائن Font.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | يضيف الخط. |
| [addFont(String file)](#addFont-java.lang.String-) | يضيف الخط. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | يضيف استبدال الخط. |
| [getDefaultFont()](#getDefaultFont--) | يحصل على الخط الافتراضي. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | يحصل على الخط. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | يقوم بتحميل جميع خطوط TrueType من المجلد المحدد إلى المجموعة الداخلية. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


يضيف الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | الدفق الذي يحتوي على الخط. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


يضيف الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | java.lang.String | المسار إلى الملف الذي يحتوي على الخط. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


يضيف استبدال الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مستبدل | java.lang.String | اسم الخط المستبدل. |
| استبدال | java.lang.String | اسم خط الاستبدال. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


يحصل على الخط الافتراضي.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


يحصل على الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontName | java.lang.String | اسم الخط. |

**Returns:**
java.awt.Font - الخط.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


يقوم بتحميل جميع خطوط TrueType من المجلد المحدد إلى المجموعة الداخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مجلد | java.lang.String | المجلد الذي يحتوي على الخطوط. |

