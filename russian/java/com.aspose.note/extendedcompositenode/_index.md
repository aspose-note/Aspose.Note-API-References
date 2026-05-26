---
title: "ExtendedCompositeNode"
second_title: "Справочник API Aspose.Note for Java"
description: "Объединяет несколько экземпляров IExtendedApsNode."
type: docs
weight: 29
url: /ru/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Объединяет несколько экземпляров `IExtendedApsNode`.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Инициализирует новый экземпляр класса `ExtendedCompositeNode`. |
## Методы

| Метод | Описание |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Добавляет `extendedApsNode` во внутренний список узлов. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Добавляет этот узел к заданному `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Применяет плоскостное преобразование, перемещая узел в плоскостях x и y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Применяет масштабирование к узлу. |
| [getApsNodes()](#getApsNodes--) | Получает все экземпляры `IExtendedApsNode`, объединённые в этом `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Создаёт полную копию этого узла. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Инициализирует новый экземпляр класса `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Добавляет `extendedApsNode` во внутренний список узлов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Получает все экземпляры `IExtendedApsNode`, объединённые в этом `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Создаёт полную копию этого узла.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
