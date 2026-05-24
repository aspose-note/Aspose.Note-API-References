---
title: "ExtendedApsPath"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Wrapper für den Standard‑ApsPath dar, der einige Zeichenverhalten erweitert."
type: docs
weight: 28
url: /de/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Stellt einen Wrapper für den standardmäßigen ApsPath dar, der das Zeichenverhalten erweitert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Initialisiert eine neue Instanz der `ExtendedApsPath`‑Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Fügt diesen Knoten dem angegebenen `compositeNode` hinzu. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Wendet Skalierung auf den Knoten an. |
| [getBottom()](#getBottom--) | Gibt den unteren Rand zurück. |
| [getCopy()](#getCopy--) | Erstellt eine vollständige Kopie dieses Knotens. |
| [getTop()](#getTop--) | Ermittelt den oberen Teil. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Initialisiert eine neue Instanz der `ExtendedApsPath`‑Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Der Aps-Pfad. |

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


Wendet Skalierung auf den Knoten an.

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
### getTop() {#getTop--}
```
public float getTop()
```


Ermittelt den oberen Teil.

**Returns:**
float
