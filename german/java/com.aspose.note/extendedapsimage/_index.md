---
title: "ExtendedApsImage"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Wrapper für das standardmäßige ApsImage dar, der das Zeichenverhalten erweitert."
type: docs
weight: 25
url: /de/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Stellt einen Wrapper für das standardmäßige ApsImage dar, der das Zeichenverhalten erweitert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Initialisiert eine neue Instanz der `ExtendedApsImage`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Fügt diesen Knoten dem angegebenen `compositeNode` hinzu. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Wendet Skalierung auf das Bild an. |
| [getBottom()](#getBottom--) | Gibt den unteren Rand zurück. |
| [getCopy()](#getCopy--) | Erstellt eine vollständige Kopie dieses Knotens. |
| [getOrigin()](#getOrigin--) | Ermittelt den Ursprung. |
| [getSize()](#getSize--) | Ermittelt die Größe. |
| [getTop()](#getTop--) | Ermittelt den oberen Teil. |
| [isBackground()](#isBackground--) | Liest, ob das Bild ein Hintergrundbild ist. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Initialisiert eine neue Instanz der `ExtendedApsImage`-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | Das Bild. |

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


Wendet Skalierung auf das Bild an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| scaleTransform | float | Der Skalierungsfaktor für die Transformation. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Gibt den unteren Rand zurück.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Erstellt eine vollständige Kopie dieses Knotens.

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
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Liest, ob das Bild ein Hintergrundbild ist.

**Returns:**
boolean
