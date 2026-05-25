---
title: "ExtendedApsImage"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un wrapper per il classico ApsImage che estende parte del comportamento di disegno."
type: docs
weight: 25
url: /it/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Rappresenta un wrapper per l'ApsImage standard, che estende parte del comportamento di disegno.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Inizializza una nuova istanza della classe `ExtendedApsImage`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Aggiunge questo nodo al `compositeNode` fornito. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applica la trasformazione del piano, spostando il nodo nei piani x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applica lo scaling all'immagine. |
| [getBottom()](#getBottom--) | Ottiene il valore inferiore. |
| [getCopy()](#getCopy--) | Crea una copia completa di questo nodo. |
| [getOrigin()](#getOrigin--) | Ottiene l'origine. |
| [getSize()](#getSize--) | Ottiene le dimensioni. |
| [getTop()](#getTop--) | Ottiene la parte superiore. |
| [isBackground()](#isBackground--) | Ottiene se l'immagine è un'immagine di sfondo. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Inizializza una nuova istanza della classe `ExtendedApsImage`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | L'immagine. |

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


Applica lo scaling all'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| scaleTransform | float | Il fattore di scala per la trasformazione. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Ottiene il valore inferiore.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Crea una copia completa di questo nodo.

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
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Ottiene se l'immagine è un'immagine di sfondo.

**Returns:**
boolean
