---
title: "ExtendedCompositeNode"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Combine plusieurs instances de IExtendedApsNode."
type: docs
weight: 29
url: /fr/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Combine plusieurs instances de `IExtendedApsNode`.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Initialise une nouvelle instance de la classe `ExtendedCompositeNode`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Ajoute `extendedApsNode` à la liste interne des nœuds. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Ajoute ce nœud au `compositeNode` donné. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applique une transformation de plan, déplaçant le nœud dans les plans x et y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applique un redimensionnement au nœud. |
| [getApsNodes()](#getApsNodes--) | Obtient toutes les instances `IExtendedApsNode` combinées dans ce `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Crée une copie complète de ce nœud. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Initialise une nouvelle instance de la classe `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Ajoute `extendedApsNode` à la liste interne des nœuds.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Ajoute ce nœud au `compositeNode` donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Applique une transformation de plan, déplaçant le nœud dans les plans x et y.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Applique un redimensionnement au nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| scaleTransform | float | Le facteur d'échelle pour la transformation. |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Obtient toutes les instances `IExtendedApsNode` combinées dans ce `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Crée une copie complète de ce nœud.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
