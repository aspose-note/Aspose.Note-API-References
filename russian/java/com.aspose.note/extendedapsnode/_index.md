---
title: "ExtendedApsNode"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет обёртку для стандартного ApsNode, которая расширяет часть поведения отрисовки."
type: docs
weight: 26
url: /ru/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Представляет обёртку для стандартного ApsNode, которая расширяет часть поведения рисования.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Добавляет этот узел к заданному `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Применяет плоскостное преобразование, перемещая узел в плоскостях x и y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Применяет масштабирование к узлу. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Получает или задаёт координату y нижней части узла. |
| [getCopy()](#getCopy--) | Создаёт полную копию этого узла. |
| [getOrigin()](#getOrigin--) | Получает или задает начало узла. |
| [getSize()](#getSize--) | Получает или задает размер узла. |
| [getTop()](#getTop--) | Получает или задает координату y верхней части узла. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Добавляет этот узел к заданному `compositeNode`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Применяет плоскостное преобразование, перемещая узел в плоскостях x и y.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Применяет масштабирование к узлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| scaleTransform | float | Коэффициент масштабирования для преобразования. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Получает или задаёт координату y нижней части узла.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Создаёт полную копию этого узла.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Получает или задает начало узла.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Получает или задает размер узла.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Получает или задает координату y верхней части узла.

**Returns:**
float
