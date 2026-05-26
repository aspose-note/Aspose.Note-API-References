---
title: "ExtendedApsGlyphs"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un contenedor para ApsGlyphs estándar que extiende parte del comportamiento de dibujo."
type: docs
weight: 24
url: /es/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Representa un contenedor para ApsGlyphs estándar, que extiende parte del comportamiento de dibujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Inicializa una nueva instancia de la clase `ExtendedApsGlyphs`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Agrega este nodo al `compositeNode` dado. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Aplica una transformación de plano, moviendo el nodo en los planos x e y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Aplica escalado a los glifos. |
| [getBottom()](#getBottom--) | Obtiene la parte inferior de los glifos. |
| [getCopy()](#getCopy--) | Obtiene una copia de los glifos. |
| [getOrigin()](#getOrigin--) | Obtiene el origen. |
| [getSize()](#getSize--) | Obtiene el tamaño. |
| [getTop()](#getTop--) | Obtiene la parte superior. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Inicializa una nueva instancia de la clase `ExtendedApsGlyphs`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Un glifo aps original. |

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


Aplica escalado a los glifos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| scaleTransform | float | El factor de escala para la transformación. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Obtiene la parte inferior de los glifos.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Obtiene una copia de los glifos.

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
