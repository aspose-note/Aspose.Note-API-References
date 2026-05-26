---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note for Java API-referentie"
description: "Combineert meerdere IExtendedApsNode-instanties."
type: docs
weight: 29
url: /nl/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Combineert verschillende `IExtendedApsNode`-instanties.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Initialiseert een nieuw exemplaar van de `ExtendedCompositeNode`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Voegt `extendedApsNode` toe aan de interne lijst met knooppunten. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Voegt dit knooppunt toe aan de gegeven `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Past een vlaktransformatie toe, waarbij het knooppunt in de x- en y-vlakken wordt verplaatst. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Past schaalvergroting toe op het knooppunt. |
| [getApsNodes()](#getApsNodes--) | Haalt alle `IExtendedApsNode`-instanties op die zijn gecombineerd in deze `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Maakt een volledige kopie van dit knooppunt. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Initialiseert een nieuw exemplaar van de `ExtendedCompositeNode`-klasse.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Voegt `extendedApsNode` toe aan de interne lijst met knooppunten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Haalt alle `IExtendedApsNode`-instanties op die zijn gecombineerd in deze `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Maakt een volledige kopie van dit knooppunt.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
