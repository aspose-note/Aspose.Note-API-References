---
title: "ExtendedApsNode"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un contenedor para un ApsNode estándar que extiende parte del comportamiento de dibujo."
type: docs
weight: 26
url: /es/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Representa un contenedor para ApsNode estándar, que extiende parte del comportamiento de dibujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Agrega este nodo al `compositeNode` dado. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Aplica una transformación de plano, moviendo el nodo en los planos x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Aplica escalado al nodo. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Obtiene o establece la coordenada y de la parte inferior del nodo. |
| [getCopy()](#getCopy--) | Crea una copia completa de este nodo. |
| [getOrigin()](#getOrigin--) | Obtiene o establece el origen del nodo. |
| [getSize()](#getSize--) | Obtiene o establece el tamaño del nodo. |
| [getTop()](#getTop--) | Obtiene o establece la coordenada y de la parte superior del nodo. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Agrega este nodo al `compositeNode` dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Aplica una transformación de plano, moviendo el nodo en los planos x e y.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Aplica escalado al nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| scaleTransform | float | El factor de escala para la transformación. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Obtiene o establece la coordenada y de la parte inferior del nodo.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Crea una copia completa de este nodo.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Obtiene o establece el origen del nodo.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Obtiene o establece el tamaño del nodo.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Obtiene o establece la coordenada y de la parte superior del nodo.

**Returns:**
float
