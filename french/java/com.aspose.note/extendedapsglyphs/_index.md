---
title: "ExtendedApsGlyphs"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un wrapper pour les ApsGlyphs standard qui étend certains comportements de dessin."
type: docs
weight: 24
url: /fr/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Représente un wrapper pour les ApsGlyphs standard, qui étend une partie du comportement de dessin.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Initialise une nouvelle instance de la classe `ExtendedApsGlyphs`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Ajoute ce nœud au `compositeNode` donné. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applique une transformation de plan, déplaçant le nœud dans les plans x et y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applique une mise à l'échelle aux glyphes. |
| [getBottom()](#getBottom--) | Obtient le bas des glyphes. |
| [getCopy()](#getCopy--) | Obtient la copie des glyphes. |
| [getOrigin()](#getOrigin--) | Obtient l'origine. |
| [getSize()](#getSize--) | Obtient la taille. |
| [getTop()](#getTop--) | Obtient le haut. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Initialise une nouvelle instance de la classe `ExtendedApsGlyphs`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Un glyphe aps original. |

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


Applique une mise à l'échelle aux glyphes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| scaleTransform | float | Le facteur d'échelle pour la transformation. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Obtient le bas des glyphes.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Obtient la copie des glyphes.

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
