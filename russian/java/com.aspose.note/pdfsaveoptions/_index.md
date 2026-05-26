---
title: "PdfSaveOptions"
second_title: "Справочник API Aspose.Note for Java"
description: "Позволяет указать дополнительные параметры при рендеринге страниц документа в PDF."
type: docs
weight: 77
url: /ru/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Позволяет указать дополнительные параметры при рендеринге страниц документа в PDF.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Инициализирует новый экземпляр класса `PdfSaveOptions`. |
## Методы

| Метод | Описание |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Получает тип сжатия, применяемый к изображениям в PDF‑файле. |
| [getJpegQuality()](#getJpegQuality--) | Получает значение, определяющее качество JPEG‑изображений в PDF‑документе. |
| [getPageSettings()](#getPageSettings--) | Получает или задает параметры страницы для каждой страницы в документе. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Получает или задает алгоритм, используемый для разбиения страниц. |
| [setImageCompression(int value)](#setImageCompression-int-) | Задает тип сжатия, применяемый к изображениям в PDF‑файле. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Задает значение, определяющее качество JPEG‑изображений в PDF‑документе. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Получает или задает параметры страницы для каждой страницы в документе. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Получает или задает алгоритм, используемый для разбиения страниц. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Инициализирует новый экземпляр класса `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Получает тип сжатия, применяемый к изображениям в PDF‑файле.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Получает значение, определяющее качество JPEG‑изображений в PDF‑документе. Значение может варьироваться от 0 до 100, где 0 означает наихудшее качество, но максимальное сжатие, а 100 — лучшее качество, но минимальное сжатие.

--------------------

Значение по умолчанию — 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Получает или задает параметры страницы для каждой страницы в документе. По умолчанию зависит от CurrentUICulture, \*US культуры используют настройки Letter, остальные — настройки A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Получает или задает алгоритм, используемый для разбиения страниц.

Значение: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Задает тип сжатия, применяемый к изображениям в PDF‑файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Задает значение, определяющее качество JPEG‑изображений в PDF‑документе. Значение может варьироваться от 0 до 100, где 0 означает наихудшее качество, но максимальное сжатие, а 100 — лучшее качество, но минимальное сжатие.

--------------------

Значение по умолчанию — 90.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Получает или задает параметры страницы для каждой страницы в документе. По умолчанию зависит от CurrentUICulture, \*US культуры используют настройки Letter, остальные — настройки A4.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Получает или задает алгоритм, используемый для разбиения страниц.

Значение: `PageSplittingAlgorithm`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

