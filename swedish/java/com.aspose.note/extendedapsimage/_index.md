---
title: "ExtendedApsImage"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en wrapper för den standard ApsImage som utökar viss ritbeteende."
type: docs
weight: 25
url: /sv/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Representerar en wrapper för standard-ApsImage, som utökar viss ritbeteende.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Initierar en ny instans av klassen `ExtendedApsImage`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Lägger till den här noden i den givna `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Tillämpar plantransform, flyttar noden i x‑ och y‑planen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Tillämpar skalning på bilden. |
| [getBottom()](#getBottom--) | Hämtar botten. |
| [getCopy()](#getCopy--) | Skapar en fullständig kopia av den här noden. |
| [getOrigin()](#getOrigin--) | Hämtar ursprunget. |
| [getSize()](#getSize--) | Hämtar storleken. |
| [getTop()](#getTop--) | Hämtar toppen. |
| [isBackground()](#isBackground--) | Hämtar om bilden är en bakgrundsbild. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Initierar en ny instans av klassen `ExtendedApsImage`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | Bilden. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Lägger till den här noden i den givna `compositeNode`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Tillämpar plantransform, flyttar noden i x‑ och y‑planen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Tillämpar skalning på bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| scaleTransform | float | Skalfaktorn för transformationen. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Hämtar botten.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Skapar en fullständig kopia av den här noden.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Hämtar ursprunget.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Hämtar storleken.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Hämtar toppen.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Hämtar om bilden är en bakgrundsbild.

**Returns:**
boolean
