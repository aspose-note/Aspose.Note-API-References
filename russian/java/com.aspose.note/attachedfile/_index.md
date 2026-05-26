---
title: "AttachedFile"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет вложенный файл."
type: docs
weight: 11
url: /ru/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Представляет вложенный файл.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Инициализирует новый экземпляр класса `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Инициализирует новый экземпляр класса `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Инициализирует новый экземпляр класса `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Инициализирует новый экземпляр класса `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Инициализирует новый экземпляр класса `AttachedFile`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getAlignment()](#getAlignment--) | Получает выравнивание. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Получает или задает тело альтернативного текста для значка вложенного файла. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Получает или задает заголовок альтернативного текста для значка вложенного файла. |
| [getBytes()](#getBytes--) | Получает двоичные данные встроенного файла. |
| [getExtension()](#getExtension--) | Получает расширение встроенного файла. |
| [getFileName()](#getFileName--) | Получает имя встроенного файла. |
| [getFilePath()](#getFilePath--) | Получает путь к оригинальному файлу. |
| [getHeight()](#getHeight--) | Получает оригинальную высоту значка встроенного файла. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Получает горизонтальное смещение. |
| [getIcon()](#getIcon--) | Получает двоичные данные значка, связанного со встроенным файлом. |
| [getIconExtension()](#getIconExtension--) | Получает расширение значка. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает время последнего изменения. |
| [getMaxHeight()](#getMaxHeight--) | Получает максимальную высоту для отображения встроенного значка файла. |
| [getMaxWidth()](#getMaxWidth--) | Получает максимальную ширину для отображения встроенного значка файла. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Получает данные об ошибке, произошедшей при доступе к файлу. |
| [getTags()](#getTags--) | Получает список тегов прикреплённого файла. |
| [getText()](#getText--) | Получает текстовое представление встроенного файла. |
| [getVerticalOffset()](#getVerticalOffset--) | Получает вертикальное смещение. |
| [getWidth()](#getWidth--) | Получает исходную ширину встроенного значка файла. |
| [isPrintout()](#isPrintout--) | Получает значение, указывающее, является ли просмотр файла печатной копией. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Получает значение, указывающее, был ли размер значка явно изменён пользователем. |
| [setAlignment(int value)](#setAlignment-int-) | Устанавливает выравнивание. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Получает или задает тело альтернативного текста для значка вложенного файла. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Получает или задает заголовок альтернативного текста для значка вложенного файла. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Устанавливает горизонтальное смещение. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Устанавливает время последнего изменения. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Устанавливает максимальную высоту для отображения встроенного значка файла. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Устанавливает максимальную ширину для отображения встроенного значка файла. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Устанавливает значение, указывающее, является ли просмотр файла печатной копией. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Устанавливает значение, указывающее, был ли размер значка явно изменён пользователем. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает текстовое представление встроенного файла. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Устанавливает вертикальное смещение. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Инициализирует новый экземпляр класса `AttachedFile`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Строка, содержащая путь к файлу, из которого создаётся `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Инициализирует новый экземпляр класса `AttachedFile`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Строка, содержащая путь к файлу, из которого создаётся `AttachedFile`. |
| icon | java.io.InputStream | Значок для прикреплённого файла. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Инициализирует новый экземпляр класса `AttachedFile`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя вложенного файла. |
| attachedFileStream | java.io.InputStream | Поток, содержащий байты вложенного файла. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Инициализирует новый экземпляр класса `AttachedFile`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя вложенного файла. |
| attachedFileStream | java.io.InputStream | Поток, содержащий байты вложенного файла. |
| icon | java.io.InputStream | Значок для прикреплённого файла. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Формат значка вложенного файла. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Инициализирует новый экземпляр класса `AttachedFile`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Получает выравнивание.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Получает или задает тело альтернативного текста для значка вложенного файла.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Получает или задает заголовок альтернативного текста для значка вложенного файла.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Получает двоичные данные встроенного файла.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Получает расширение встроенного файла.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Получает имя встроенного файла.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Получает путь к оригинальному файлу.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Получает оригинальную высоту значка встроенного файла.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Получает горизонтальное смещение.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Получает двоичные данные значка, связанного со встроенным файлом.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Получает расширение значка.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает время последнего изменения.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Получает максимальную высоту для отображения встроенного значка файла.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Получает максимальную ширину для отображения встроенного значка файла.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Получает данные об ошибке, произошедшей при доступе к файлу.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Получает список тегов прикреплённого файла.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Получает текстовое представление вложенного файла. Строка НЕ ДОЛЖНА содержать символы со значением 10 (перевод строки) или 13 (возврат каретки).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Получает вертикальное смещение.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Получает исходную ширину встроенного значка файла.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Получает значение, указывающее, является ли просмотр файла печатной копией.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Получает значение, указывающее, был ли размер значка явно изменён пользователем.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Устанавливает выравнивание.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int | Значение Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Получает или задает тело альтернативного текста для значка вложенного файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Получает или задает заголовок альтернативного текста для значка вложенного файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Устанавливает горизонтальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float | Значение Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Устанавливает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date | Значение Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Устанавливает максимальную высоту для отображения встроенного значка файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float | Значение максимальной высоты. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Устанавливает максимальную ширину для отображения встроенного значка файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float | Значение максимальной ширины. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Устанавливает значение, указывающее, является ли просмотр файла печатной копией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | Новое значение. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Устанавливает значение, указывающее, был ли размер значка явно изменён пользователем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | Новое значение. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Устанавливает текстовое представление вложенного файла. Строка НЕ ДОЛЖНА содержать символы со значением 10 (перевод строки) или 13 (возврат каретки).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Устанавливает вертикальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float | Значение Offset. |

