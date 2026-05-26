---
title: "ExtendedApsNode"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en wrapper för en standard‑ApsNode som utökar en del av ritningsbeteendet."
type: docs
weight: 26
url: /sv/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Representerar en wrapper för en standard-ApsNode, som utökar viss ritbeteende.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Lägger till den här noden i den givna `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Tillämpar plantransform, flyttar noden i x‑ och y‑planen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Tillämpar skalning på noden. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Hämtar eller anger y‑koordinaten för nodens botten. |
| [getCopy()](#getCopy--) | Skapar en fullständig kopia av den här noden. |
| [getOrigin()](#getOrigin--) | Hämtar eller anger ursprunget för noden. |
| [getSize()](#getSize--) | Hämtar eller anger storleken på noden. |
| [getTop()](#getTop--) | Hämtar eller anger y-koordinaten för nodens topp. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Lägger till den här noden i den givna `compositeNode`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Tillämpar plantransform, flyttar noden i x‑ och y‑planen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Tillämpar skalning på noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| scaleTransform | float | Skalfaktorn för transformationen. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Hämtar eller anger y‑koordinaten för nodens botten.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Skapar en fullständig kopia av den här noden.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Hämtar eller anger ursprunget för noden.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Hämtar eller anger storleken på noden.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Hämtar eller anger y-koordinaten för nodens topp.

**Returns:**
float
