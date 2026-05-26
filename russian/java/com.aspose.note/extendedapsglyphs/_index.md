---
title: "ExtendedApsGlyphs"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет обёртку для стандартных ApsGlyphs, которая расширяет некоторые аспекты поведения отрисовки."
type: docs
weight: 24
url: /ru/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Представляет обёртку для стандартных ApsGlyphs, которая расширяет часть поведения рисования.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Инициализирует новый экземпляр класса `ExtendedApsGlyphs`. |
## Методы

| Метод | Описание |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Добавляет этот узел к заданному `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Применяет плоскостное преобразование, перемещая узел в плоскостях x и y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Применяет масштабирование к глифам. |
| [getBottom()](#getBottom--) | Получает нижнюю границу глифов. |
| [getCopy()](#getCopy--) | Получает копию глифов. |
| [getOrigin()](#getOrigin--) | Получает начало координат. |
| [getSize()](#getSize--) | Получает размер. |
| [getTop()](#getTop--) | Получает верхнюю границу. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Инициализирует новый экземпляр класса `ExtendedApsGlyphs`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Оригинальные глифы aps. |

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


Применяет масштабирование к глифам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| scaleTransform | float | Коэффициент масштабирования для преобразования. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Получает нижнюю границу глифов.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Получает копию глифов.

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
