---
title: "Изображение"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет изображение."
type: docs
weight: 33
url: /ru/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Представляет изображение.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Инициализирует новый экземпляр класса `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Инициализирует новый экземпляр класса `Image`. |
| [Image()](#Image--) | Инициализирует новый экземпляр класса `Image`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getAlignment()](#getAlignment--) | Получает выравнивание. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Получает тело альтернативного текста для изображения. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Получает заголовок альтернативного текста для изображения. |
| [getBytes()](#getBytes--) | Получает хранилище данных изображения. |
| [getFileName()](#getFileName--) | Получает имя файла. |
| [getFilePath()](#getFilePath--) | Получает путь к файлу изображения. |
| [getFormat()](#getFormat--) | Получает формат изображения. |
| [getHeight()](#getHeight--) | Получает высоту. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Получает горизонтальное смещение. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Получает гиперссылку, связанную с изображением. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает время последнего изменения. |
| [getOriginalHeight()](#getOriginalHeight--) | Получает оригинальную высоту. |
| [getOriginalWidth()](#getOriginalWidth--) | Получает оригинальную ширину. |
| [getTags()](#getTags--) | Получает список всех тегов изображения. |
| [getVerticalOffset()](#getVerticalOffset--) | Получает вертикальное смещение. |
| [getWidth()](#getWidth--) | Получает ширину. |
| [isBackground()](#isBackground--) | Получает, является ли изображение фоновым. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Заменяет текущие данные изображения данными из предоставленного объекта Image. |
| [setAlignment(int value)](#setAlignment-int-) | Устанавливает выравнивание. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Устанавливает тело альтернативного текста для изображения. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Устанавливает заголовок альтернативного текста для изображения. |
| [setBackground(boolean value)](#setBackground-boolean-) | Получает, является ли изображение фоновым. |
| [setHeight(float value)](#setHeight-float-) | Устанавливает высоту. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Устанавливает горизонтальное смещение. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Устанавливает гиперссылку, связанную с изображением. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Устанавливает время последнего изменения. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Устанавливает вертикальное смещение. |
| [setWidth(float value)](#setWidth-float-) | Устанавливает ширину. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Инициализирует новый экземпляр класса `Image`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Строка, содержащая путь к файлу, из которого создаётся `Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Инициализирует новый экземпляр класса `Image`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя изображения. |
| imageStream | java.io.InputStream | Поток, содержащий изображение. |

### Image() {#Image--}
```
public Image()
```


Инициализирует новый экземпляр класса `Image`.

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


Получает тело альтернативного текста для изображения.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Получает заголовок альтернативного текста для изображения.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Получает хранилище данных изображения.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Получает имя файла.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Получает путь к файлу изображения.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Получает формат изображения.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Получает высоту. Это реальная высота изображения в документе MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Получает горизонтальное смещение.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Получает гиперссылку, связанную с изображением.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает время последнего изменения.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Получает оригинальную высоту. Это оригинальная ширина изображения до изменения размера.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Получает оригинальную ширину. Это оригинальная ширина изображения до изменения размера.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Получает список всех тегов изображения.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Получает вертикальное смещение.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Получает ширину. Это реальная ширина изображения в документе MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Получает, является ли изображение фоновым.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Заменяет текущие данные изображения данными из предоставленного объекта Image.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Устанавливает выравнивание.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Устанавливает тело альтернативного текста для изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Устанавливает заголовок альтернативного текста для изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Получает, является ли изображение фоновым.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Устанавливает высоту. Это реальная высота изображения в документе MS OneNote.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Устанавливает горизонтальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Устанавливает гиперссылку, связанную с изображением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Устанавливает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Устанавливает вертикальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Устанавливает ширину. Это реальная ширина изображения в документе MS OneNote.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

