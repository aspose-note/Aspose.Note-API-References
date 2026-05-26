---
title: "ExtendedApsImage"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет обёртку для стандартного ApsImage, который расширяет часть поведения рисования."
type: docs
weight: 25
url: /ru/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Представляет обёртку для стандартного ApsImage, которая расширяет часть поведения рисования.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Инициализирует новый экземпляр класса `ExtendedApsImage`. |
## Методы

| Метод | Описание |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Добавляет этот узел к заданному `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Применяет плоскостное преобразование, перемещая узел в плоскостях x и y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Применяет масштабирование к изображению. |
| [getBottom()](#getBottom--) | Возвращает нижнюю границу. |
| [getCopy()](#getCopy--) | Создаёт полную копию этого узла. |
| [getOrigin()](#getOrigin--) | Получает начало координат. |
| [getSize()](#getSize--) | Получает размер. |
| [getTop()](#getTop--) | Получает верхнюю границу. |
| [isBackground()](#isBackground--) | Получает, является ли изображение фоновым. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Инициализирует новый экземпляр класса `ExtendedApsImage`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | Изображение. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Добавляет этот узел к заданному `compositeNode`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Применяет плоскостное преобразование, перемещая узел в плоскостях x и y.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Применяет масштабирование к изображению.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| scaleTransform | float | Коэффициент масштабирования для преобразования. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Возвращает нижнюю границу.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Создаёт полную копию этого узла.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Получает начало координат.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Получает размер.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Получает верхнюю границу.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Получает, является ли изображение фоновым.

**Returns:**
boolean
