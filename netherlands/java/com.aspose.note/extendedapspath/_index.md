---
title: "ExtendedApsPath"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een wrapper voor de standaard ApsPath voor die een deel van het teken‑gedrag uitbreidt."
type: docs
weight: 28
url: /nl/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Stelt een wrapper voor het standaard ApsPath voor, die een deel van het teken-gedrag uitbreidt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Initialiseert een nieuw exemplaar van de `ExtendedApsPath`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Voegt dit knooppunt toe aan de gegeven `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Past schaalvergroting toe op het knooppunt. |
| [getBottom()](#getBottom--) | Haalt de onderkant op. |
| [getCopy()](#getCopy--) | Maakt een volledige kopie van dit knooppunt. |
| [getTop()](#getTop--) | Haalt de bovenkant op. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Initialiseert een nieuw exemplaar van de `ExtendedApsPath`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Het aps-pad. |

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


Past schaalvergroting toe op het knooppunt.

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
### getTop() {#getTop--}
```
public float getTop()
```


Haalt de bovenkant op.

**Returns:**
float
