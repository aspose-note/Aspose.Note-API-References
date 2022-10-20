---
title: FontsSubsystem
second_title: Aspose.Note for Java API Reference
description: Base class implementing com.aspose.note.IFontsSubsystem interface.
type: docs
weight: 11
url: /java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Base class implementing com.aspose.note.IFontsSubsystem interface. Provides functionality for default font and font's substitutions. Override com.aspose.note.FontsSubsystem.fetchFontFamily protected member function in a derived class to implement logic for retrieving of Font object.
## Methods

| Method | Description |
| --- | --- |
| [getDefaultFont()](#getDefaultFont--) | Gets default font. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Adds font substitution. |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Adds the font. |
| [addFont(String file)](#addFont-java.lang.String-) | Adds the font. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Loads all TrueType fonts from specified folder to internal collection. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Gets font. |
### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Gets default font.

**Returns:**
java.awt.Font
### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Adds font substitution.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| substituted | java.lang.String | The substituted font name. |
| substitution | java.lang.String | The substitution font name. |

### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Adds the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream containing the font. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Adds the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.lang.String | The path to the file containing the font. |

### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Loads all TrueType fonts from specified folder to internal collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| folder | java.lang.String | The folder containing fonts. |

### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Gets font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | The font name. |

**Returns:**
java.awt.Font - The Font.
