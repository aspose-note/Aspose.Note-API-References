---
title: "ExtendedApsPath"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет обёртку для стандартного ApsPath, которая расширяет часть поведения рисования."
type: docs
weight: 28
url: /ru/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Представляет обёртку для стандартного ApsPath, которая расширяет часть поведения рисования.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Инициализирует новый экземпляр класса `ExtendedApsPath`. |
## Методы

| Метод | Описание |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Добавляет этот узел к заданному `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Применяет плоскостное преобразование, перемещая узел в плоскостях x и y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Применяет масштабирование к узлу. |
| [getBottom()](#getBottom--) | Возвращает нижнюю границу. |
| [getCopy()](#getCopy--) | Создаёт полную копию этого узла. |
| [getTop()](#getTop--) | Получает верхнюю границу. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Инициализирует новый экземпляр класса `ExtendedApsPath`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Путь aps. |

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


Применяет масштабирование к узлу.

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
### getTop() {#getTop--}
```
public float getTop()
```


Получает верхнюю границу.

**Returns:**
float
