---
title: "NumberList"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет нумерованный или маркированный список."
type: docs
weight: 64
url: /ru/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Представляет нумерованный или маркированный список.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Инициализирует новый экземпляр класса `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Инициализирует новый экземпляр класса `NumberList`. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Определяет, равен ли указанный объект текущему объекту. |
| [equals(Object obj)](#equals-java.lang.Object-) | Определяет, равен ли указанный объект текущему объекту. |
| [getFont()](#getFont--) | Получает или задает имя шрифта. |
| [getFontColor()](#getFontColor--) | Получает или задает цвет шрифта. |
| [getFontSize()](#getFontSize--) | Получает или задает размер шрифта. |
| [getFormat()](#getFormat--) | Получает или задает формат заголовка строки. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает или задает время последнего изменения. |
| [getNumberFormat()](#getNumberFormat--) | Получает или задает числовой формат, используемый для группы автоматически нумерованных объектов. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Получает заголовок нумерованного списка. |
| [getRestart()](#getRestart--) | Получает или задает числовое значение, которое переопределяет автоматическое числовое значение элемента списка. |
| [hashCode()](#hashCode--) | Служит хеш-функцией для типа. |
| [isBold()](#isBold--) | Получает или задает значение, указывающее, является ли стиль текста полужирным. |
| [isItalic()](#isItalic--) | Получает или задает значение, указывающее, является ли стиль текста курсивом. |
| [setBold(boolean value)](#setBold-boolean-) | Получает или задает значение, указывающее, является ли стиль текста полужирным. |
| [setFont(String value)](#setFont-java.lang.String-) | Получает или задает имя шрифта. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Получает или задает цвет шрифта. |
| [setFontSize(int value)](#setFontSize-int-) | Получает или задает размер шрифта. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Получает или задает формат заголовка строки. |
| [setItalic(boolean value)](#setItalic-boolean-) | Получает или задает значение, указывающее, является ли стиль текста курсивом. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Получает или задает время последнего изменения. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Получает или задает числовой формат, используемый для группы автоматически нумерованных объектов. |
| [setRestart(int value)](#setRestart-int-) | Получает или задает числовое значение, которое переопределяет автоматическое числовое значение элемента списка. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Инициализирует новый экземпляр класса `NumberList`. Этот экземпляр представляет маркированный список.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Символ, представляющий маркер. |
| font | java.lang.String | Шрифт для маркера. |
| fontSize | int | Размер шрифта для маркера. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Инициализирует новый экземпляр класса `NumberList`. Этот экземпляр представляет нумерованный список.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| format | java.lang.String | Формат нумерованного заголовка. |
| numberFormat | byte | Формат числа в заголовке. |
| font | java.lang.String | Шрифт для нумерованного заголовка. |
| fontSize | int | Размер шрифта для нумерованного заголовка. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Определяет, равен ли указанный объект текущему объекту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Объект. |

**Returns:**
boolean - Тип `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Определяет, равен ли указанный объект текущему объекту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Объект. |

**Returns:**
boolean - Тип `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Получает или задает имя шрифта.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Получает или задает цвет шрифта.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Получает или задает размер шрифта.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Получает или задает формат заголовка строки. Для маркированных списков представляет символ маркера.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает или задает время последнего изменения.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Получает или задает формат чисел, используемый для группы автоматически нумерованных объектов. Должен быть null для маркированных списков.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Получает заголовок нумерованного списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sequenceNumber | int | Последовательный номер в нумерованном списке. |

**Returns:**
java.lang.String - Строковое представление указанного последовательного номера.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Получает или задает числовое значение, которое переопределяет автоматическое числовое значение элемента списка.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Служит хеш-функцией для типа.

**Returns:**
int - Тип `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Получает или задает значение, указывающее, является ли стиль текста полужирным.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Получает или задает значение, указывающее, является ли стиль текста курсивом.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Получает или задает значение, указывающее, является ли стиль текста полужирным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Получает или задает имя шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Получает или задает цвет шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Получает или задает размер шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Получает или задает формат заголовка строки. Для маркированных списков представляет символ маркера.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Получает или задает значение, указывающее, является ли стиль текста курсивом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Получает или задает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Получает или задает формат чисел, используемый для группы автоматически нумерованных объектов. Должен быть null для маркированных списков.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Получает или задает числовое значение, которое переопределяет автоматическое числовое значение элемента списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

