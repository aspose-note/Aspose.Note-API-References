---
title: "ExtendedApsNode"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un wrapper per un ApsNode standard che estende parte del comportamento di disegno."
type: docs
weight: 26
url: /it/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Rappresenta un wrapper per un ApsNode standard, che estende parte del comportamento di disegno.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Aggiunge questo nodo al `compositeNode` fornito. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applica la trasformazione del piano, spostando il nodo nei piani x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applica la scalatura al nodo. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Ottiene o imposta la coordinata y della parte inferiore del nodo. |
| [getCopy()](#getCopy--) | Crea una copia completa di questo nodo. |
| [getOrigin()](#getOrigin--) | Ottiene o imposta l'origine del nodo. |
| [getSize()](#getSize--) | Ottiene o imposta la dimensione del nodo. |
| [getTop()](#getTop--) | Ottiene o imposta la coordinata y della parte superiore del nodo. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Aggiunge questo nodo al `compositeNode` fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Applica la trasformazione del piano, spostando il nodo nei piani x e y.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Applica la scalatura al nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| scaleTransform | float | Il fattore di scala per la trasformazione. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Ottiene o imposta la coordinata y della parte inferiore del nodo.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Crea una copia completa di questo nodo.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Ottiene o imposta l'origine del nodo.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Ottiene o imposta la dimensione del nodo.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Ottiene o imposta la coordinata y della parte superiore del nodo.

**Returns:**
float
