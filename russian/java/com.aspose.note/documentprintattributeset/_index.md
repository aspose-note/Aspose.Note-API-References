---
title: "DocumentPrintAttributeSet"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет вспомогательный класс с удобным для пользователя интерфейсом к AttributeSet."
type: docs
weight: 21
url: /ru/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Представляет вспомогательный класс с удобным для пользователя интерфейсом к AttributeSet.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Инициализирует новый экземпляр `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Инициализирует новый экземпляр `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Инициализирует новый экземпляр `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Инициализирует новый экземпляр `DocumentPrintAttributeSet`. |
## Методы

| Метод | Описание |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Устанавливает значение, указывающее, собран ли документ. |
| [setCopies(int value)](#setCopies-int-) | Устанавливает количество копий для печати. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Устанавливает параметр принтера для двусторонней печати. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Устанавливает ориентацию страницы. |
| [setPrintRange(int page)](#setPrintRange-int-) | Устанавливает отдельную страницу для печати. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Устанавливает диапазон страниц для печати. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Имя используемого принтера. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Имя используемого принтера. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Инициализирует новый экземпляр `DocumentPrintAttributeSet`. По умолчанию печатаются все страницы документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| копии | int | Количество копий документа для печати. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Инициализирует новый экземпляр `DocumentPrintAttributeSet`. По умолчанию печатаются все страницы документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | Имя принтера. |
| копии | int | Количество копий документа для печати. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Инициализирует новый экземпляр `DocumentPrintAttributeSet`. По умолчанию печатается только одна копия каждой страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | Имя принтера. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Инициализирует новый экземпляр `DocumentPrintAttributeSet`. По умолчанию печатается только одна копия каждой страницы.

### getCopies() {#getCopies--}
```
public int getCopies()
```




**Returns:**
int
### getLandscape() {#getLandscape--}
```
public boolean getLandscape()
```




**Returns:**
boolean
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```




**Returns:**
java.lang.String
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


Устанавливает значение, указывающее, собран ли документ.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | true эквивалентно настройке SheetCollate.COLLATED, false эквивалентно настройке SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Устанавливает количество копий для печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int | Количество копий для печати. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Устанавливает параметр принтера для двусторонней печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | true эквивалентно настройке Sides.DUPLEX, false эквивалентно настройке Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Устанавливает ориентацию страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | true эквивалентно настройке OrientationRequested.LANDSCAPE, false эквивалентно настройке OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Устанавливает отдельную страницу для печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| страница | int | Страница для печати. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Устанавливает диапазон страниц для печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| от | int | Первая страница. |
| до | int | Последняя страница. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Имя используемого принтера.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | Имя принтера. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Имя используемого принтера.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | Имя принтера. |
| локаль | java.util.Locale | локаль printerName. |

