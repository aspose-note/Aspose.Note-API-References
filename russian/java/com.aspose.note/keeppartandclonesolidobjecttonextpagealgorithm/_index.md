---
title: "KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Справочник API Aspose.Note for Java"
description: "Добавляет верхнюю часть объектов в нижнюю часть страницы и клонирует весь объект на следующую страницу, если он не помещается на оригинальной странице."
type: docs
weight: 42
url: /ru/java/com.aspose.note/keeppartandclonesolidobjecttonextpagealgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm extends PageSplittingAlgorithm
```

Добавляет верхнюю часть объекта в нижнюю часть страницы и клонирует весь объект на следующую страницу, если он не помещается на исходной странице.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm()](#KeepPartAndCloneSolidObjectToNextPageAlgorithm--) | Инициализирует новый экземпляр класса `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, используя ограничение высоты по умолчанию для клонированной части. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)](#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-) | Инициализирует новый экземпляр класса `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, используя конкретное ограничение высоты для клонированной части. |
## Поля

| Поле | Описание |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | Максимальный размер клонированной части по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | Получает ограничение высоты клонированной части. |
### KeepPartAndCloneSolidObjectToNextPageAlgorithm() {#KeepPartAndCloneSolidObjectToNextPageAlgorithm--}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm()
```


Инициализирует новый экземпляр класса `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, используя ограничение высоты по умолчанию для клонированной части.

### KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart) {#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)
```


Инициализирует новый экземпляр класса `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, используя конкретное ограничение высоты для клонированной части.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| heightLimitOfClonedPart | float | Максимальная высота клонированной части. |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


Максимальный размер клонированной части по умолчанию.

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


Получает ограничение высоты клонированной части.

**Returns:**
float
