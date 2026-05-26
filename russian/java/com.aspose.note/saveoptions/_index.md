---
title: "SaveOptions"
second_title: "Справочник API Aspose.Note for Java"
description: "Абстрактный базовый класс, представляющий параметры сохранения документа для определённого формата."
type: docs
weight: 85
url: /ru/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Абстрактный базовый класс, представляющий параметры сохранения документа для определённого формата.
## Методы

| Метод | Описание |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Получает или задает настройки шрифта, используемые при сохранении |
| [getPageCount()](#getPageCount--) | Получает или задает количество страниц для сохранения. |
| [getPageIndex()](#getPageIndex--) | Получает или задает индекс первой страницы для сохранения. |
| [getSaveFormat()](#getSaveFormat--) | Получает или задает формат, в котором сохраняется документ. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Получает или задает настройки шрифта, используемые при сохранении |
| [setPageCount(int value)](#setPageCount-int-) | Получает или задает количество страниц для сохранения. |
| [setPageIndex(int value)](#setPageIndex-int-) | Получает или задает индекс первой страницы для сохранения. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Получает или задает настройки шрифта, используемые при сохранении

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Получает или задает количество страниц для сохранения. По умолчанию \{@link int\#Int32Extensions.MaxValue\}, что означает, что все страницы документа будут отрисованы.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Получает или задает индекс первой страницы для сохранения. По умолчанию 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает или задает формат, в котором сохраняется документ.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Получает или задает настройки шрифта, используемые при сохранении

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Получает или задает количество страниц для сохранения. По умолчанию \{@link int\#Int32Extensions.MaxValue\}, что означает, что все страницы документа будут отрисованы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Получает или задает индекс первой страницы для сохранения. По умолчанию 0.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

