---
title: "ExtendedApsNode"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een wrapper voor een standaard ApsNode voor die een deel van het teken gedrag uitbreidt."
type: docs
weight: 26
url: /nl/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Stelt een wrapper voor een standaard ApsNode voor, die een deel van het teken-gedrag uitbreidt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Voegt dit knooppunt toe aan de gegeven `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Past schaalvergroting toe op het knooppunt. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Haalt op of stelt de y-coördinaat van de onderkant van het knooppunt in. |
| [getCopy()](#getCopy--) | Maakt een volledige kopie van dit knooppunt. |
| [getOrigin()](#getOrigin--) | Haalt de oorsprong van het knooppunt op of stelt deze in. |
| [getSize()](#getSize--) | Haalt de grootte van het knooppunt op of stelt deze in. |
| [getTop()](#getTop--) | Haalt de y-coördinaat van de bovenkant van het knooppunt op of stelt deze in. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Voegt dit knooppunt toe aan de gegeven `compositeNode`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Past schaalvergroting toe op het knooppunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| scaleTransform | float | De schaalfactor voor de transformatie. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Haalt op of stelt de y-coördinaat van de onderkant van het knooppunt in.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Maakt een volledige kopie van dit knooppunt.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Haalt de oorsprong van het knooppunt op of stelt deze in.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Haalt de grootte van het knooppunt op of stelt deze in.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Haalt de y-coördinaat van de bovenkant van het knooppunt op of stelt deze in.

**Returns:**
float
