---
title: "ExtendedApsImage"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un contenedor para el ApsImage estándar que extiende parte del comportamiento de dibujo."
type: docs
weight: 25
url: /es/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Representa un contenedor para ApsImage estándar, que extiende parte del comportamiento de dibujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Inicializa una nueva instancia de la clase `ExtendedApsImage`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Agrega este nodo al `compositeNode` dado. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Aplica una transformación de plano, moviendo el nodo en los planos x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Aplica escalado a la imagen. |
| [getBottom()](#getBottom--) | Obtiene la parte inferior. |
| [getCopy()](#getCopy--) | Crea una copia completa de este nodo. |
| [getOrigin()](#getOrigin--) | Obtiene el origen. |
| [getSize()](#getSize--) | Obtiene el tamaño. |
| [getTop()](#getTop--) | Obtiene la parte superior. |
| [isBackground()](#isBackground--) | Obtiene si la imagen es una imagen de fondo. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Inicializa una nueva instancia de la clase `ExtendedApsImage`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | La imagen. |

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


Aplica escalado a la imagen.

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
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Obtiene el origen.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Obtiene el tamaño.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Obtiene la parte superior.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Obtiene si la imagen es una imagen de fondo.

**Returns:**
boolean
