---
title: "Imagen"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa una Imagen."
type: docs
weight: 33
url: /es/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Representa una Imagen.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Inicializa una nueva instancia de la clase `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Inicializa una nueva instancia de la clase `Image`. |
| [Image()](#Image--) | Inicializa una nueva instancia de la clase `Image`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getAlignment()](#getAlignment--) | Obtiene la alineación. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Obtiene un cuerpo de texto alternativo para la imagen. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Obtiene un título del texto alternativo para la imagen. |
| [getBytes()](#getBytes--) | Obtiene el almacén de datos de la imagen. |
| [getFileName()](#getFileName--) | Obtiene el nombre del archivo. |
| [getFilePath()](#getFilePath--) | Obtiene la ruta al archivo de imagen. |
| [getFormat()](#getFormat--) | Obtiene el formato de la imagen. |
| [getHeight()](#getHeight--) | Obtiene la altura. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtiene el desplazamiento horizontal. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Obtiene el hipervínculo asociado con la imagen. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene la hora de la última modificación. |
| [getOriginalHeight()](#getOriginalHeight--) | Obtiene la altura original. |
| [getOriginalWidth()](#getOriginalWidth--) | Obtiene el ancho original. |
| [getTags()](#getTags--) | Obtiene la lista de todas las etiquetas de una imagen. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtiene el desplazamiento vertical. |
| [getWidth()](#getWidth--) | Obtiene el ancho. |
| [isBackground()](#isBackground--) | Obtiene si la imagen es una imagen de fondo. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Reemplaza los datos de la imagen actual con los datos del objeto Image proporcionado. |
| [setAlignment(int value)](#setAlignment-int-) | Establece la alineación. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Establece un cuerpo de texto alternativo para la imagen. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Establece un título del texto alternativo para la imagen. |
| [setBackground(boolean value)](#setBackground-boolean-) | Obtiene si la imagen es una imagen de fondo. |
| [setHeight(float value)](#setHeight-float-) | Establece la altura. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Establece el desplazamiento horizontal. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Establece el hipervínculo asociado con la imagen. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Establece la hora de última modificación. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Establece el desplazamiento vertical. |
| [setWidth(float value)](#setWidth-float-) | Establece el ancho. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Inicializa una nueva instancia de la clase `Image`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | Una cadena que contiene la ruta al archivo desde el cual crear el `Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Inicializa una nueva instancia de la clase `Image`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | Un nombre de la imagen. |
| imageStream | java.io.InputStream | Un flujo que contiene la imagen. |

### Image() {#Image--}
```
public Image()
```


Inicializa una nueva instancia de la clase `Image`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Obtiene la alineación.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Obtiene un cuerpo de texto alternativo para la imagen.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Obtiene un título del texto alternativo para la imagen.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Obtiene el almacén de datos de la imagen.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Obtiene el nombre del archivo.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Obtiene la ruta al archivo de imagen.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Obtiene el formato de la imagen.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Obtiene la altura. Esta es la altura real de la imagen en el documento MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Obtiene el desplazamiento horizontal.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Obtiene el hipervínculo asociado con la imagen.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene la hora de la última modificación.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Obtiene la altura original. Esta es la anchura original de la imagen, antes de redimensionar.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Obtiene la anchura original. Esta es la anchura original de la imagen, antes de redimensionar.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtiene la lista de todas las etiquetas de una imagen.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Obtiene el desplazamiento vertical.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Obtiene la anchura. Esta es la anchura real de la imagen en el documento MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Obtiene si la imagen es una imagen de fondo.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Reemplaza los datos de la imagen actual con los datos del objeto Image proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Establece la alineación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Establece un cuerpo de texto alternativo para la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Establece un título del texto alternativo para la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Obtiene si la imagen es una imagen de fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Establece la altura. Esta es la altura real de la imagen en el documento MS OneNote.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Establece el desplazamiento horizontal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Establece el hipervínculo asociado con la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Establece la hora de última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Establece el desplazamiento vertical.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Establece la anchura. Esta es la anchura real de la imagen en el documento MS OneNote.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

