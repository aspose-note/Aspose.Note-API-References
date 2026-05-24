---
title: "ExtendedApsGlyphs"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Wrapper für standardmäßige ApsGlyphs dar, der das Zeichenverhalten erweitert."
type: docs
weight: 24
url: /de/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Stellt einen Wrapper für standardmäßige ApsGlyphs dar, der das Zeichenverhalten erweitert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Initialisiert eine neue Instanz der `ExtendedApsGlyphs`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Fügt diesen Knoten dem angegebenen `compositeNode` hinzu. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Wendet Skalierung auf die Glyphen an. |
| [getBottom()](#getBottom--) | Ermittelt den unteren Teil der Glyphen. |
| [getCopy()](#getCopy--) | Ermittelt die Kopie der Glyphen. |
| [getOrigin()](#getOrigin--) | Ermittelt den Ursprung. |
| [getSize()](#getSize--) | Ermittelt die Größe. |
| [getTop()](#getTop--) | Ermittelt den oberen Teil. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Initialisiert eine neue Instanz der `ExtendedApsGlyphs`-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Ein originales APS-Glyph. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Fügt diesen Knoten dem angegebenen `compositeNode` hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Wendet Skalierung auf die Glyphen an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| scaleTransform | float | Der Skalierungsfaktor für die Transformation. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Ermittelt den unteren Teil der Glyphen.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Ermittelt die Kopie der Glyphen.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Ermittelt den Ursprung.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Ermittelt die Größe.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Ermittelt den oberen Teil.

**Returns:**
float
