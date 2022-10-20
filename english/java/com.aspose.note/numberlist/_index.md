---
title: NumberList
second_title: Aspose.Note for Java API Reference
description: Represents the numbered or bulleted list.
type: docs
weight: 49
url: /java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Represents the numbered or bulleted list.
## Constructors

| Constructor | Description |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Initializes a new instance of the  NumberList  class. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Initializes a new instance of the  NumberList  class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [getFont()](#getFont--) | Gets or sets the name of the font. |
| [setFont(String value)](#setFont-java.lang.String-) | Gets or sets the name of the font. |
| [getNumberFormat()](#getNumberFormat--) | Gets or sets the number format used for a group of automatically numbered objects. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Gets or sets the number format used for a group of automatically numbered objects. |
| [getFormat()](#getFormat--) | Gets or sets the format of the line header. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Gets or sets the format of the line header. |
| [isBold()](#isBold--) | Gets or sets a value indicating whether the text style is bold. |
| [setBold(boolean value)](#setBold-boolean-) | Gets or sets a value indicating whether the text style is bold. |
| [isItalic()](#isItalic--) | Gets or sets a value indicating whether the text style is italic. |
| [setItalic(boolean value)](#setItalic-boolean-) | Gets or sets a value indicating whether the text style is italic. |
| [getFontSize()](#getFontSize--) | Gets or sets the font size. |
| [setFontSize(int value)](#setFontSize-int-) | Gets or sets the font size. |
| [getFontColor()](#getFontColor--) | Gets or sets the font color. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Gets or sets the font color. |
| [getRestart()](#getRestart--) | Gets or sets the numeric value that overrides the automatic number value of the list item. |
| [setRestart(int value)](#setRestart-int-) | Gets or sets the numeric value that overrides the automatic number value of the list item. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Gets the numbered list header. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether the specified object is equal to the current object. |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Determines whether the specified object is equal to the current object. |
| [hashCode()](#hashCode--) | Serves as a hash function for the type. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Initializes a new instance of the  NumberList  class. This instance represents a bulleted list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | A symbol which represents a bullet. |
| font | java.lang.String | A font for the bullet. |
| fontSize | int | A font size for the bullet. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Initializes a new instance of the  NumberList  class. This instance represents a numbered list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | java.lang.String | The format of the numbered header. |
| numberFormat | byte | The format of the number in header. |
| font | java.lang.String | A font for the numbered header. |
| fontSize | int | A font size for the numbered header. |

### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getFont() {#getFont--}
```
public String getFont()
```


Gets or sets the name of the font.

**Returns:**
java.lang.String
### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Gets or sets the name of the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Gets or sets the number format used for a group of automatically numbered objects. Should be null for bulleted lists.

**Returns:**
java.lang.Byte
### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Gets or sets the number format used for a group of automatically numbered objects. Should be null for bulleted lists.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Byte |  |

### getFormat() {#getFormat--}
```
public String getFormat()
```


Gets or sets the format of the line header. For bulleted lists represents a bullet symbol.

**Returns:**
java.lang.String
### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Gets or sets the format of the line header. For bulleted lists represents a bullet symbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### isBold() {#isBold--}
```
public boolean isBold()
```


Gets or sets a value indicating whether the text style is bold.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Gets or sets a value indicating whether the text style is bold.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Gets or sets a value indicating whether the text style is italic.

**Returns:**
boolean
### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Gets or sets a value indicating whether the text style is italic.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Gets or sets the font size.

**Returns:**
int
### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Gets or sets the font size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Gets or sets the font color.

**Returns:**
java.awt.Color
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Gets or sets the font color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### getRestart() {#getRestart--}
```
public int getRestart()
```


Gets or sets the numeric value that overrides the automatic number value of the list item.

**Returns:**
int
### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Gets or sets the numeric value that overrides the automatic number value of the list item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Gets the numbered list header.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sequenceNumber | int | The sequence number in the numbered list. |

**Returns:**
java.lang.String - A string representation of the specified sequence number.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the specified object is equal to the current object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object. |

**Returns:**
boolean - The  bool .
### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Determines whether the specified object is equal to the current object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | The object. |

**Returns:**
boolean - The  bool .
### hashCode() {#hashCode--}
```
public int hashCode()
```


Serves as a hash function for the type.

**Returns:**
int - The  int .
