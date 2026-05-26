---
title: "RichText"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет форматированный текст."
type: docs
weight: 82
url: /ru/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Представляет форматированный текст.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [RichText()](#RichText--) | Инициализирует новый экземпляр класса [RichText](../../com.aspose.note/richtext). |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [append(String value)](#append-java.lang.String-) | Добавляет строку к последнему диапазону текста. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Добавляет строку в конец. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Добавляет строку в начало первого диапазона текста. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Добавляет строку в начало. |
| [clear()](#clear--) | Очищает содержимое этого экземпляра. |
| [getAlignment()](#getAlignment--) | Получает выравнивание. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает время последнего изменения. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Получает межстрочный интервал. |
| [getParagraphStyle()](#getParagraphStyle--) | Получает стиль абзаца. |
| [getSpaceAfter()](#getSpaceAfter--) | Получает минимальное количество пространства после. |
| [getSpaceBefore()](#getSpaceBefore--) | Получает минимальное количество пространства перед. |
| [getStyles()](#getStyles--) | Получает стили. |
| [getTags()](#getTags--) | Получает список всех тегов абзаца. |
| [getText()](#getText--) | Получает текст. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Возвращает нулевой индекс первого вхождения указанного символа Unicode в этой строке. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Возвращает нулевой индекс первого вхождения указанного символа Unicode в этой строке. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Возвращает нулевой индекс первого вхождения указанного символа в этом экземпляре. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Возвращает нулевой индекс первого вхождения указанной строки в этом экземпляре. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Возвращает нулевой индекс первого вхождения указанной строки в этом экземпляре. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Возвращает нулевой индекс первого вхождения указанной строки в этом экземпляре. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Возвращает нулевой индекс первого вхождения указанной строки в текущем экземпляре. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Возвращает нулевой индекс первого вхождения указанной строки в текущем экземпляре. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Возвращает нулевой индекс первого вхождения указанной строки в текущем экземпляре. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Вставляет указанную строку в указанную позицию индекса в этом экземпляре. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Вставляет указанную строку с указанным стилем в указанную позицию индекса в этом экземпляре. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Удаляет все символы в текущем экземпляре, начиная с указанной позиции и до последней позиции. |
| [remove(int startIndex, int count)](#remove-int-int-) | Удаляет указанное количество символов в текущем экземпляре, начиная с указанной позиции. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Заменяет все вхождения указанного символа Unicode в этом экземпляре другим указанным символом Unicode. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой в указанном стиле. |
| [setAlignment(int value)](#setAlignment-int-) | Устанавливает выравнивание. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Устанавливает время последнего изменения. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Устанавливает межстрочный интервал. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Устанавливает стиль абзаца. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Устанавливает минимальное количество пространства после. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Устанавливает минимальное количество пространства перед. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает текст. |
| [trim()](#trim--) | Удаляет все начальные и конечные пробельные символы. |
| [trim(char trimChar)](#trim-char-) | Удаляет все начальные и конечные вхождения символа. |
| [trim(char[] trimChars)](#trim-char...-) | Удаляет все начальные и конечные вхождения набора символов, указанных в массиве. |
| [trimEnd()](#trimEnd--) | Удаляет все конечные пробельные символы. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Удаляет все конечные вхождения символа. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Удаляет все конечные вхождения набора символов, указанных в массиве. |
| [trimStart()](#trimStart--) | Удаляет все начальные пробельные символы. |
| [trimStart(char trimChar)](#trimStart-char-) | Удаляет все начальные вхождения указанного символа. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Удаляет все начальные вхождения набора символов, указанных в массиве. |
### RichText() {#RichText--}
```
public RichText()
```


Инициализирует новый экземпляр класса [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Добавляет строку к последнему диапазону текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Добавленное значение. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Добавляет строку в конец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Добавленное значение. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Стиль добавленной строки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Добавляет строку в начало первого диапазона текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Добавленное значение. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Добавляет строку в начало.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Добавленное значение. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Стиль добавленной строки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Очищает содержимое этого экземпляра.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Получает выравнивание.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает время последнего изменения.

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


Получает межстрочный интервал.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Получает стиль абзаца. Эти настройки используются, если в коллекции [getStyles](../../com.aspose.note/richtext\#getStyles) нет соответствующего объекта TextStyle, либо этот объект не указывает необходимую настройку.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Получает минимальное количество пространства после.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Получает минимальное количество пространства перед.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Получает стили.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Получает список всех тегов абзаца.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Получает текст. Строка НЕ ДОЛЖНА содержать любые символы со значением 10 (перевод строки).

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


Возвращает нулевой индекс первого вхождения указанного символа Unicode в этой строке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char | Значение. |

**Returns:**
int - Тип `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Возвращает нулевой индекс первого вхождения указанного символа Unicode в этой строке. Поиск начинается с указанной позиции символа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char | Значение. |
| startIndex | int | Начальная позиция поиска |

**Returns:**
int - Тип `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Возвращает нулевой индекс первого вхождения указанного символа в этом экземпляре. Поиск начинается с указанной позиции символа и проверяет указанное количество позиций символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char | Значение. |
| startIndex | int | Начальная позиция поиска |
| count | int | Количество. |

**Returns:**
int - Тип `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Возвращает нулевой индекс первого вхождения указанной строки в этом экземпляре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение. |

**Returns:**
int - Тип `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Возвращает индекс, начинающийся с нуля, первого вхождения указанной строки в данном экземпляре. Поиск начинается с указанной позиции символа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение. |
| startIndex | int | Начальная позиция поиска |

**Returns:**
int - Тип `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Возвращает индекс, начинающийся с нуля, первого вхождения указанной строки в данном экземпляре. Поиск начинается с указанной позиции символа и проверяет указанное количество позиций символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение. |
| startIndex | int | Начальная позиция поиска |
| count | int | Количество. |

**Returns:**
int - Тип `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Возвращает нулевой индекс первого вхождения указанной строки в текущем экземпляре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение. |
| startIndex | int | Начальная позиция поиска |
| count | int | Количество. |
| comparisonType | short | Тип поиска, используемый для указанной строки |

**Returns:**
int - Тип `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Возвращает индекс, начинающийся с нуля, первого вхождения указанной строки в текущем экземпляре. Параметр указывает тип поиска, используемый для указанной строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение. |
| comparisonType | short | Тип поиска, используемый для указанной строки |

**Returns:**
int - Тип `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Возвращает индекс, начинающийся с нуля, первого вхождения указанной строки в текущем экземпляре. Параметры указывают начальную позицию поиска в текущей строке и тип поиска, используемый для указанной строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение. |
| startIndex | int | Начальная позиция поиска |
| comparisonType | short | Тип поиска, используемый для указанной строки |

**Returns:**
int - Тип `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Вставляет указанную строку в указанную позицию индекса в этом экземпляре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальная позиция. |
| значение | java.lang.String | Значение. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Вставляет указанную строку с указанным стилем в указанную позицию индекса в этом экземпляре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальная позиция. |
| значение | java.lang.String | Значение. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Стиль. |

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


Удаляет все символы в текущем экземпляре, начиная с указанной позиции и до последней позиции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальная позиция. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Удаляет указанное количество символов в текущем экземпляре, начиная с указанной позиции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальная позиция. |
| count | int | Количество. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Заменяет все вхождения указанного символа Unicode в этом экземпляре другим указанным символом Unicode.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldChar | char | Старый символ. |
| newChar | char | Новый символ. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldValue | java.lang.String | Старое значение. |
| newValue | java.lang.String | Новое значение. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой в указанном стиле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldValue | java.lang.String | Старое значение. |
| newValue | java.lang.String | Новое значение. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Стиль нового значения. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Устанавливает выравнивание.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Устанавливает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Устанавливает межстрочный интервал.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Устанавливает стиль абзаца. Эти настройки используются, если в коллекции [getStyles](../../com.aspose.note/richtext\#getStyles) нет соответствующего объекта TextStyle, либо данный объект не указывает необходимую настройку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Устанавливает минимальное количество пространства после.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Устанавливает минимальное количество пространства перед.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Устанавливает текст. Строка НЕ ДОЛЖНА содержать любые символы со значением 10 (перевод строки).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Удаляет все начальные и конечные пробельные символы.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Удаляет все начальные и конечные вхождения символа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| trimChar | char | Символ обрезки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Удаляет все начальные и конечные вхождения набора символов, указанных в массиве.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| trimChars | char[] | Символы обрезки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Удаляет все конечные пробельные символы.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Удаляет все конечные вхождения символа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| trimChar | char | Символ обрезки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Удаляет все конечные вхождения набора символов, указанных в массиве.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| trimChars | char[] | Символы обрезки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Удаляет все начальные пробельные символы.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Удаляет все начальные вхождения указанного символа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| trimChar | char | Символ обрезки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Удаляет все начальные вхождения набора символов, указанных в массиве.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| trimChars | char[] | Символы обрезки. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
