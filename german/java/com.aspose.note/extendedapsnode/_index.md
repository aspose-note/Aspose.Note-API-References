---
title: "ExtendedApsNode"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Wrapper für einen Standard‑ApsNode dar, der einige Zeichen‑Verhaltensweisen erweitert."
type: docs
weight: 26
url: /de/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Stellt einen Wrapper für einen standardmäßigen ApsNode dar, der das Zeichenverhalten erweitert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Fügt diesen Knoten dem angegebenen `compositeNode` hinzu. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Wendet Skalierung auf den Knoten an. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Liest oder setzt die y‑Koordinate des unteren Knotens. |
| [getCopy()](#getCopy--) | Erstellt eine vollständige Kopie dieses Knotens. |
| [getOrigin()](#getOrigin--) | Ruft den Ursprung des Knotens ab oder legt ihn fest. |
| [getSize()](#getSize--) | Ruft die Größe des Knotens ab oder legt sie fest. |
| [getTop()](#getTop--) | Ruft die y‑Koordinate des Knotens oben ab oder legt sie fest. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Fügt diesen Knoten dem angegebenen `compositeNode` hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Wendet Skalierung auf den Knoten an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| scaleTransform | float | Der Skalierungsfaktor für die Transformation. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Liest oder setzt die y‑Koordinate des unteren Knotens.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Erstellt eine vollständige Kopie dieses Knotens.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Ruft den Ursprung des Knotens ab oder legt ihn fest.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Ruft die Größe des Knotens ab oder legt sie fest.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Ruft die y‑Koordinate des Knotens oben ab oder legt sie fest.

**Returns:**
float
