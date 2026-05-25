---
title: "ExtendedCompositeNode"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Combina diverse istanze di IExtendedApsNode."
type: docs
weight: 29
url: /it/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Combina diverse istanze di `IExtendedApsNode`.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Inizializza una nuova istanza della classe `ExtendedCompositeNode`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Aggiunge `extendedApsNode` all'elenco interno di nodi. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Aggiunge questo nodo al `compositeNode` fornito. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applica la trasformazione del piano, spostando il nodo nei piani x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applica la scalatura al nodo. |
| [getApsNodes()](#getApsNodes--) | Ottiene tutte le istanze di `IExtendedApsNode` combinate in questo `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Crea una copia completa di questo nodo. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Inizializza una nuova istanza della classe `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Aggiunge `extendedApsNode` all'elenco interno di nodi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Ottiene tutte le istanze di `IExtendedApsNode` combinate in questo `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Crea una copia completa di questo nodo.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
