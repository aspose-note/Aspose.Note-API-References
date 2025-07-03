---
title: RichText
second_title: Aspose.Note for Java API Reference
description: Represents a rich text.
type: docs
weight: 82
url: /java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Represents a rich text.
## Constructors

| Constructor | Description |
| --- | --- |
| [RichText()](#RichText--) | Initializes a new instance of the [RichText](../../com.aspose.note/richtext) class. |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [append(String value)](#append-java.lang.String-) | Adds a string to the last text range. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Adds a string to the end. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Adds a string to the front of the first text range. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Adds a string to the front. |
| [clear()](#clear--) | Clears content of this instance. |
| [getAlignment()](#getAlignment--) | Gets the alignment. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets the last modified time. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Gets the line spacing. |
| [getParagraphStyle()](#getParagraphStyle--) | Gets the paragraph style. |
| [getSpaceAfter()](#getSpaceAfter--) | Gets the minimum amount of space after. |
| [getSpaceBefore()](#getSpaceBefore--) | Gets the minimum amount of space before. |
| [getStyles()](#getStyles--) | Gets the styles. |
| [getTags()](#getTags--) | Gets the list of all tags of a paragraph. |
| [getText()](#getText--) | Gets the text. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Returns the zero-based index of the first occurrence of the specified Unicode character in this string. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Returns the zero-based index of the first occurrence of the specified Unicode character in this string. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Returns the zero-based index of the first occurrence of the specified character in this instance. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Returns the zero-based index of the first occurrence of the specified string in this instance. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Returns the zero-based index of the first occurrence of the specified string in this instance. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Returns the zero-based index of the first occurrence of the specified string in this instance. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Returns the zero-based index of the first occurrence of the specified string in the current instance. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Returns the zero-based index of the first occurrence of the specified string in the current instance. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Returns the zero-based index of the first occurrence of the specified string in the current instance. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Inserts a specified string at a specified index position in this instance. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Inserts a specified string with specified style at a specified index position in this instance. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Removes all the characters in the current instance, beginning at a specified position and continuing through the last position. |
| [remove(int startIndex, int count)](#remove-int-int-) | Removes specified number of characters in the current instance beginning at a specified position. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Replaces all occurrences of a specified Unicode character in this instance with another specified Unicode character. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Replaces all occurrences of a specified string in the current instance with another specified string. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Replaces all occurrences of a specified string in the current instance with another specified string in specified style. |
| [setAlignment(int value)](#setAlignment-int-) | Sets the alignment. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Sets the last modified time. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Sets the line spacing. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Sets the paragraph style. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Sets the minimum amount of space after. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Sets the minimum amount of space before. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text. |
| [trim()](#trim--) | Removes all leading and trailing white-space characters. |
| [trim(char trimChar)](#trim-char-) | Removes all leading and trailing instances of a character. |
| [trim(char[] trimChars)](#trim-char...-) | Removes all leading and trailing occurrences of a set of characters specified in an array. |
| [trimEnd()](#trimEnd--) | Removes all the trailing white-space characters. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Removes all the trailing occurrences of a character. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Removes all the trailing occurrences of a set of characters specified in an array. |
| [trimStart()](#trimStart--) | Removes all the leading white-space characters. |
| [trimStart(char trimChar)](#trimStart-char-) | Removes all the leading occurrences of a specified character. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Removes all the leading occurrences of a set of characters specified in an array. |
### RichText() {#RichText--}
```
public RichText()
```


Initializes a new instance of the [RichText](../../com.aspose.note/richtext) class.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Adds a string to the last text range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The added value. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Adds a string to the end.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The added value. |
| style | [TextStyle](../../com.aspose.note/textstyle) | The style of added string. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Adds a string to the front of the first text range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The added value. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Adds a string to the front.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The added value. |
| style | [TextStyle](../../com.aspose.note/textstyle) | The style of added string. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Clears content of this instance.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Gets the alignment.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets the last modified time.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Gets the line spacing.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Gets the paragraph style. These settings are used if there is no matching TextStyle object in [getStyles](../../com.aspose.note/richtext\#getStyles) collection either this object doesn't specify a needed setting.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Gets the minimum amount of space after.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Gets the minimum amount of space before.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Gets the styles.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of all tags of a paragraph.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Gets the text. The string MUST NOT contain any characters of the value 10 (line feed).

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Returns the zero-based index of the first occurrence of the specified Unicode character in this string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char | The value. |

**Returns:**
int - The `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Returns the zero-based index of the first occurrence of the specified Unicode character in this string. The search starts at a specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char | The value. |
| startIndex | int | The starting search position |

**Returns:**
int - The `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Returns the zero-based index of the first occurrence of the specified character in this instance. The search starts at a specified character position and examines a specified number of character positions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char | The value. |
| startIndex | int | The starting search position |
| count | int | The count. |

**Returns:**
int - The `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Returns the zero-based index of the first occurrence of the specified string in this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value. |

**Returns:**
int - The `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Returns the zero-based index of the first occurrence of the specified string in this instance. The search starts at a specified character position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value. |
| startIndex | int | The starting search position |

**Returns:**
int - The `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Returns the zero-based index of the first occurrence of the specified string in this instance. The search starts at a specified character position and examines a specified number of character positions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value. |
| startIndex | int | The starting search position |
| count | int | The count. |

**Returns:**
int - The `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Returns the zero-based index of the first occurrence of the specified string in the current instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value. |
| startIndex | int | The starting search position |
| count | int | The count. |
| comparisonType | short | The type of search to use for the specified string |

**Returns:**
int - The `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Returns the zero-based index of the first occurrence of the specified string in the current instance. A parameter specifies the type of search to use for the specified string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value. |
| comparisonType | short | The type of search to use for the specified string |

**Returns:**
int - The `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Returns the zero-based index of the first occurrence of the specified string in the current instance. Parameters specify the starting search position in the current string and the type of search to use for the specified string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value. |
| startIndex | int | The starting search position |
| comparisonType | short | The type of search to use for the specified string |

**Returns:**
int - The `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Inserts a specified string at a specified index position in this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| value | java.lang.String | The value. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Inserts a specified string with specified style at a specified index position in this instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| value | java.lang.String | The value. |
| style | [TextStyle](../../com.aspose.note/textstyle) | The style. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Removes all the characters in the current instance, beginning at a specified position and continuing through the last position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Removes specified number of characters in the current instance beginning at a specified position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| count | int | The count. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Replaces all occurrences of a specified Unicode character in this instance with another specified Unicode character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldChar | char | The old char. |
| newChar | char | The new char. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Replaces all occurrences of a specified string in the current instance with another specified string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | The old value. |
| newValue | java.lang.String | The new value. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Replaces all occurrences of a specified string in the current instance with another specified string in specified style.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | The old value. |
| newValue | java.lang.String | The new value. |
| style | [TextStyle](../../com.aspose.note/textstyle) | The style of the new value. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Sets the alignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Sets the line spacing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Sets the paragraph style. These settings are used if there is no matching TextStyle object in [getStyles](../../com.aspose.note/richtext\#getStyles) collection either this object doesn't specify a needed setting.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Sets the minimum amount of space after.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Sets the minimum amount of space before.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Sets the text. The string MUST NOT contain any characters of the value 10 (line feed).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Removes all leading and trailing white-space characters.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Removes all leading and trailing instances of a character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| trimChar | char | The trim char. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Removes all leading and trailing occurrences of a set of characters specified in an array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| trimChars | char[] | The trim chars. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Removes all the trailing white-space characters.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Removes all the trailing occurrences of a character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| trimChar | char | The trim char. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Removes all the trailing occurrences of a set of characters specified in an array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| trimChars | char[] | The trim chars. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Removes all the leading white-space characters.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Removes all the leading occurrences of a specified character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| trimChar | char | The trim char. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Removes all the leading occurrences of a set of characters specified in an array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| trimChars | char[] | The trim chars. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
