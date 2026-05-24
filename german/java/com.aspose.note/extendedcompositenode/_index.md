---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note für Java API-Referenz"
description: "Kombiniert mehrere IExtendedApsNode-Instanzen."
type: docs
weight: 29
url: /de/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Kombiniert mehrere `IExtendedApsNode`-Instanzen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Initialisiert eine neue Instanz der Klasse `ExtendedCompositeNode`. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Fügt `extendedApsNode` zur internen Liste von Knoten hinzu. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Fügt diesen Knoten dem angegebenen `compositeNode` hinzu. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Wendet eine Ebenentransformation an und bewegt den Knoten in den x‑ und y‑Ebenen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Wendet Skalierung auf den Knoten an. |
| [getApsNodes()](#getApsNodes--) | Ruft alle `IExtendedApsNode`-Instanzen ab, die in diesem `ExtendedCompositeNode` kombiniert sind. |
| [getCopy()](#getCopy--) | Erstellt eine vollständige Kopie dieses Knotens. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Initialisiert eine neue Instanz der Klasse `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Fügt `extendedApsNode` zur internen Liste von Knoten hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Ruft alle `IExtendedApsNode`-Instanzen ab, die in diesem `ExtendedCompositeNode` kombiniert sind.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Erstellt eine vollständige Kopie dieses Knotens.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
