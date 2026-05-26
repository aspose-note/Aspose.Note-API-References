---
title: "ExtendedApsPath"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un contenedor para el ApsPath estándar que extiende parte del comportamiento de dibujo."
type: docs
weight: 28
url: /es/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Representa un contenedor para ApsPath estándar, que extiende parte del comportamiento de dibujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Inicializa una nueva instancia de la clase `ExtendedApsPath`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Agrega este nodo al `compositeNode` dado. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Aplica una transformación de plano, moviendo el nodo en los planos x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Aplica escalado al nodo. |
| [getBottom()](#getBottom--) | Obtiene la parte inferior. |
| [getCopy()](#getCopy--) | Crea una copia completa de este nodo. |
| [getTop()](#getTop--) | Obtiene la parte superior. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Inicializa una nueva instancia de la clase `ExtendedApsPath`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | La ruta aps. |

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

### getBottom() {#getBottom--}
```
public float getBottom()
```


Obtiene la parte inferior.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Crea una copia completa de este nodo.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getTop() {#getTop--}
```
public float getTop()
```


Obtiene la parte superior.

**Returns:**
float
