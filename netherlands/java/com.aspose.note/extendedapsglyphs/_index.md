---
title: "ExtendedApsGlyphs"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een wrapper voor standaard ApsGlyphs voor die een deel van het teken‑gedrag uitbreidt."
type: docs
weight: 24
url: /nl/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Stelt een wrapper voor standaard ApsGlyphs voor, die een deel van het teken-gedrag uitbreidt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Initialiseert een nieuw exemplaar van de `ExtendedApsGlyphs` klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Voegt dit knooppunt toe aan de gegeven `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Past schaal toe op de glyphs. |
| [getBottom()](#getBottom--) | Haalt de onderkant van de glyphs op. |
| [getCopy()](#getCopy--) | Haalt een kopie van de glyphs op. |
| [getOrigin()](#getOrigin--) | Haalt de oorsprong op. |
| [getSize()](#getSize--) | Haalt de grootte op. |
| [getTop()](#getTop--) | Haalt de bovenkant op. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Initialiseert een nieuw exemplaar van de `ExtendedApsGlyphs` klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Een originele aps-glyfen. |

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


Past schaal toe op de glyphs.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| scaleTransform | float | De schaalfactor voor de transformatie. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Haalt de onderkant van de glyphs op.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Haalt een kopie van de glyphs op.

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
