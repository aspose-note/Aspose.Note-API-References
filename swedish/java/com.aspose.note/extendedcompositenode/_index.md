---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note for Java API-referens"
description: "Kombinerar flera IExtendedApsNode-instansers."
type: docs
weight: 29
url: /sv/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Kombinerar flera `IExtendedApsNode`-instanser.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Initierar en ny instans av klassen `ExtendedCompositeNode`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Lägger till `extendedApsNode` i den interna listan med noder. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Lägger till den här noden i den givna `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Tillämpar plantransform, flyttar noden i x‑ och y‑planen. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Tillämpar skalning på noden. |
| [getApsNodes()](#getApsNodes--) | Hämtar alla `IExtendedApsNode`-instanser som kombineras i detta `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Skapar en fullständig kopia av den här noden. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Initierar en ny instans av klassen `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Lägger till `extendedApsNode` i den interna listan med noder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Lägger till den här noden i den givna `compositeNode`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Tillämpar plantransform, flyttar noden i x‑ och y‑planen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Tillämpar skalning på noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| scaleTransform | float | Skalfaktorn för transformationen. |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Hämtar alla `IExtendedApsNode`-instanser som kombineras i detta `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Skapar en fullständig kopia av den här noden.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
