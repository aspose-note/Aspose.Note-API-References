---
title: "ExtendedApsImage"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een wrapper voor de standaard ApsImage voor die een deel van het teken‑gedrag uitbreidt."
type: docs
weight: 25
url: /nl/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Stelt een wrapper voor de standaard ApsImage voor, die een deel van het teken-gedrag uitbreidt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Initialiseert een nieuw exemplaar van de `ExtendedApsImage`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Voegt dit knooppunt toe aan de gegeven `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Past schaling toe op de afbeelding. |
| [getBottom()](#getBottom--) | Haalt de onderkant op. |
| [getCopy()](#getCopy--) | Maakt een volledige kopie van dit knooppunt. |
| [getOrigin()](#getOrigin--) | Haalt de oorsprong op. |
| [getSize()](#getSize--) | Haalt de grootte op. |
| [getTop()](#getTop--) | Haalt de bovenkant op. |
| [isBackground()](#isBackground--) | Haalt op of de afbeelding een achtergrondafbeelding is. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Initialiseert een nieuw exemplaar van de `ExtendedApsImage`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | De afbeelding. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Voegt dit knooppunt toe aan de gegeven `compositeNode`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Past schaling toe op de afbeelding.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| scaleTransform | float | De schaalfactor voor de transformatie. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Haalt de onderkant op.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Maakt een volledige kopie van dit knooppunt.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Haalt de oorsprong op.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Haalt de grootte op.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Haalt de bovenkant op.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Haalt op of de afbeelding een achtergrondafbeelding is.

**Returns:**
boolean
