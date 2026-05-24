---
title: "ExtendedApsPath"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un wrapper pour le ApsPath standard qui étend certains comportements de dessin."
type: docs
weight: 28
url: /fr/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Représente un wrapper pour le ApsPath standard, qui étend une partie du comportement de dessin.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Initialise une nouvelle instance de la classe `ExtendedApsPath`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Ajoute ce nœud au `compositeNode` donné. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applique une transformation de plan, déplaçant le nœud dans les plans x et y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applique un redimensionnement au nœud. |
| [getBottom()](#getBottom--) | Obtient le bas. |
| [getCopy()](#getCopy--) | Crée une copie complète de ce nœud. |
| [getTop()](#getTop--) | Obtient le haut. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Initialise une nouvelle instance de la classe `ExtendedApsPath`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Le chemin aps. |

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

### getBottom() {#getBottom--}
```
public float getBottom()
```


Obtient le bas.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Crée une copie complète de ce nœud.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getTop() {#getTop--}
```
public float getTop()
```


Obtient le haut.

**Returns:**
float
