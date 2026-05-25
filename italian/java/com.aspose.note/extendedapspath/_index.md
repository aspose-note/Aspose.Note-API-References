---
title: "ExtendedApsPath"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un wrapper per il classico ApsPath che estende alcuni comportamenti di disegno."
type: docs
weight: 28
url: /it/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Rappresenta un wrapper per l'ApsPath standard, che estende parte del comportamento di disegno.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Inizializza una nuova istanza della classe `ExtendedApsPath`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Aggiunge questo nodo al `compositeNode` fornito. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applica la trasformazione del piano, spostando il nodo nei piani x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applica la scalatura al nodo. |
| [getBottom()](#getBottom--) | Ottiene il valore inferiore. |
| [getCopy()](#getCopy--) | Crea una copia completa di questo nodo. |
| [getTop()](#getTop--) | Ottiene la parte superiore. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Inizializza una nuova istanza della classe `ExtendedApsPath`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Il percorso aps. |

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


Applica la scalatura al nodo.

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
### getTop() {#getTop--}
```
public float getTop()
```


Ottiene la parte superiore.

**Returns:**
float
