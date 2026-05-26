---
title: "ExtendedCompositeNode"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Combina varias instancias de IExtendedApsNode."
type: docs
weight: 29
url: /es/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Combina varias instancias de `IExtendedApsNode`.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Inicializa una nueva instancia de la clase `ExtendedCompositeNode`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Agrega `extendedApsNode` a la lista interna de nodos. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Agrega este nodo al `compositeNode` dado. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Aplica una transformación de plano, moviendo el nodo en los planos x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Aplica escalado al nodo. |
| [getApsNodes()](#getApsNodes--) | Obtiene todas las instancias `IExtendedApsNode` combinadas en este `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Crea una copia completa de este nodo. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Inicializa una nueva instancia de la clase `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Agrega `extendedApsNode` a la lista interna de nodos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Agrega este nodo al `compositeNode` dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Aplica una transformación de plano, moviendo el nodo en los planos x e y.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Aplica escalado al nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| scaleTransform | float | El factor de escala para la transformación. |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Obtiene todas las instancias `IExtendedApsNode` combinadas en este `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Crea una copia completa de este nodo.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
