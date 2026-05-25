---
title: "ExtendedApsGlyphs"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un wrapper per gli ApsGlyphs standard che estende alcuni comportamenti di disegno."
type: docs
weight: 24
url: /it/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Rappresenta un wrapper per gli ApsGlyphs standard, che estende parte del comportamento di disegno.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Inizializza una nuova istanza della classe `ExtendedApsGlyphs`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Aggiunge questo nodo al `compositeNode` fornito. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applica la trasformazione del piano, spostando il nodo nei piani x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applica la scalatura ai glifi. |
| [getBottom()](#getBottom--) | Ottiene la parte inferiore dei glifi. |
| [getCopy()](#getCopy--) | Ottiene la copia dei glifi. |
| [getOrigin()](#getOrigin--) | Ottiene l'origine. |
| [getSize()](#getSize--) | Ottiene le dimensioni. |
| [getTop()](#getTop--) | Ottiene la parte superiore. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Inizializza una nuova istanza della classe `ExtendedApsGlyphs`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Un originale glifo aps. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Aggiunge questo nodo al `compositeNode` fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Applica la trasformazione del piano, spostando il nodo nei piani x e y.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Applica la scalatura ai glifi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| scaleTransform | float | Il fattore di scala per la trasformazione. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Ottiene la parte inferiore dei glifi.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Ottiene la copia dei glifi.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Ottiene l'origine.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Ottiene le dimensioni.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Ottiene la parte superiore.

**Returns:**
float
