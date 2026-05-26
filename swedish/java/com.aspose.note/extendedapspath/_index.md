---
title: "ExtendedApsPath"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en wrapper för den standard ApsPath som utökar viss ritningsbeteende."
type: docs
weight: 28
url: /sv/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Representerar en wrapper för standard-ApsPath, som utökar viss ritbeteende.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Initierar en ny instans av klassen `ExtendedApsPath`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Lägger till den här noden i den givna `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Tillämpar plantransform, flyttar noden i x‑ och y‑planen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Tillämpar skalning på noden. |
| [getBottom()](#getBottom--) | Hämtar botten. |
| [getCopy()](#getCopy--) | Skapar en fullständig kopia av den här noden. |
| [getTop()](#getTop--) | Hämtar toppen. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Initierar en ny instans av klassen `ExtendedApsPath`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Aps-sökvägen. |

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


Tillämpar skalning på noden.

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
### getTop() {#getTop--}
```
public float getTop()
```


Hämtar toppen.

**Returns:**
float
