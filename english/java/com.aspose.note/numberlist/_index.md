---
title: NumberList
second_title: Aspose.Note for Java API Reference
description: Represents the numbered or bulleted list.
type: docs
weight: 64
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
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Determines whether the specified object is equal to the current object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether the specified object is equal to the current object. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Gets or sets the name of the font. |
| [getFontColor()](#getFontColor--) | Gets or sets the font color. |
| [getFontSize()](#getFontSize--) | Gets or sets the font size. |
| [getFormat()](#getFormat--) | Gets or sets the format of the line header. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getNumberFormat()](#getNumberFormat--) | Gets or sets the number format used for a group of automatically numbered objects. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Gets the numbered list header. |
| [getRestart()](#getRestart--) | Gets or sets the numeric value that overrides the automatic number value of the list item. |
| [hashCode()](#hashCode--) | Serves as a hash function for the type. |
| [isBold()](#isBold--) | Gets or sets a value indicating whether the text style is bold. |
| [isItalic()](#isItalic--) | Gets or sets a value indicating whether the text style is italic. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBold(boolean value)](#setBold-boolean-) | Gets or sets a value indicating whether the text style is bold. |
| [setFont(String value)](#setFont-java.lang.String-) | Gets or sets the name of the font. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Gets or sets the font color. |
| [setFontSize(int value)](#setFontSize-int-) | Gets or sets the font size. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Gets or sets the format of the line header. |
| [setItalic(boolean value)](#setItalic-boolean-) | Gets or sets a value indicating whether the text style is italic. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Gets or sets the number format used for a group of automatically numbered objects. |
| [setRestart(int value)](#setRestart-int-) | Gets or sets the numeric value that overrides the automatic number value of the list item. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public String getFont()
```


Gets or sets the name of the font.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Gets or sets the font color.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Gets or sets the font size.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Gets or sets the format of the line header. For bulleted lists represents a bullet symbol.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Gets or sets the number format used for a group of automatically numbered objects. Should be null for bulleted lists.

**Returns:**
java.lang.Byte
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
### getRestart() {#getRestart--}
```
public int getRestart()
```


Gets or sets the numeric value that overrides the automatic number value of the list item.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Serves as a hash function for the type.

**Returns:**
int - The  int .
### isBold() {#isBold--}
```
public boolean isBold()
```


Gets or sets a value indicating whether the text style is bold.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Gets or sets a value indicating whether the text style is italic.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Gets or sets a value indicating whether the text style is bold.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Gets or sets the name of the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Gets or sets the font color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Gets or sets the font size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Gets or sets the format of the line header. For bulleted lists represents a bullet symbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Gets or sets a value indicating whether the text style is italic.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Gets or sets the number format used for a group of automatically numbered objects. Should be null for bulleted lists.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Gets or sets the numeric value that overrides the automatic number value of the list item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

