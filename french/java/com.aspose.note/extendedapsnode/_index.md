---
title: "ExtendedApsNode"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un wrapper pour un ApsNode standard qui étend certains comportements de dessin."
type: docs
weight: 26
url: /fr/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Représente un wrapper pour un ApsNode standard, qui étend une partie du comportement de dessin.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Ajoute ce nœud au `compositeNode` donné. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applique une transformation de plan, déplaçant le nœud dans les plans x et y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applique un redimensionnement au nœud. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Obtient ou définit la coordonnée y du bas du nœud. |
| [getCopy()](#getCopy--) | Crée une copie complète de ce nœud. |
| [getOrigin()](#getOrigin--) | Obtient ou définit l'origine du nœud. |
| [getSize()](#getSize--) | Obtient ou définit la taille du nœud. |
| [getTop()](#getTop--) | Obtient ou définit la coordonnée y du haut du nœud. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Ajoute ce nœud au `compositeNode` donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Applique une transformation de plan, déplaçant le nœud dans les plans x et y.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Applique un redimensionnement au nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| scaleTransform | float | Le facteur d'échelle pour la transformation. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Obtient ou définit la coordonnée y du bas du nœud.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Crée une copie complète de ce nœud.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Obtient ou définit l'origine du nœud.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Obtient ou définit la taille du nœud.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Obtient ou définit la coordonnée y du haut du nœud.

**Returns:**
float
