---
title: "ExtendedApsImage"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un wrapper pour le ApsImage standard qui étend certains comportements de dessin."
type: docs
weight: 25
url: /fr/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Représente un wrapper pour l'ApsImage standard, qui étend une partie du comportement de dessin.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Initialise une nouvelle instance de la classe `ExtendedApsImage`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Ajoute ce nœud au `compositeNode` donné. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applique une transformation de plan, déplaçant le nœud dans les plans x et y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applique un redimensionnement à l'image. |
| [getBottom()](#getBottom--) | Obtient le bas. |
| [getCopy()](#getCopy--) | Crée une copie complète de ce nœud. |
| [getOrigin()](#getOrigin--) | Obtient l'origine. |
| [getSize()](#getSize--) | Obtient la taille. |
| [getTop()](#getTop--) | Obtient le haut. |
| [isBackground()](#isBackground--) | Obtient si l'image est une image d'arrière-plan. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Initialise une nouvelle instance de la classe `ExtendedApsImage`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | L'image. |

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


Applique un redimensionnement à l'image.

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
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Obtient l'origine.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Obtient la taille.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Obtient le haut.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Obtient si l'image est une image d'arrière-plan.

**Returns:**
boolean
