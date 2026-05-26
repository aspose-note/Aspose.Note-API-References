---
title: "ExtendedApsGlyphs"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en wrapper för standard‑ApsGlyphs som utökar viss ritbeteende."
type: docs
weight: 24
url: /sv/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Representerar en wrapper för standard-ApsGlyphs, som utökar viss ritbeteende.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Initierar en ny instans av klassen `ExtendedApsGlyphs`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Lägger till den här noden i den givna `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Tillämpar plantransform, flyttar noden i x‑ och y‑planen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Tillämpar skalning på glyferna. |
| [getBottom()](#getBottom--) | Hämtar botten av glyferna. |
| [getCopy()](#getCopy--) | Hämtar en kopia av glyferna. |
| [getOrigin()](#getOrigin--) | Hämtar ursprunget. |
| [getSize()](#getSize--) | Hämtar storleken. |
| [getTop()](#getTop--) | Hämtar toppen. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Initierar en ny instans av klassen `ExtendedApsGlyphs`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | En original aps-glyf. |

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


Tillämpar skalning på glyferna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| scaleTransform | float | Skalfaktorn för transformationen. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Hämtar botten av glyferna.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Hämtar en kopia av glyferna.

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
