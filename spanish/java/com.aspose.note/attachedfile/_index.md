---
title: "AttachedFile"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un archivo adjunto."
type: docs
weight: 11
url: /es/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Representa un archivo adjunto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Inicializa una nueva instancia de la clase `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Inicializa una nueva instancia de la clase `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Inicializa una nueva instancia de la clase `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Inicializa una nueva instancia de la clase `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Inicializa una nueva instancia de la clase `AttachedFile`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getAlignment()](#getAlignment--) | Obtiene la alineación. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Obtiene o establece un cuerpo de texto alternativo para el ícono del archivo adjunto. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Obtiene o establece un título de texto alternativo para el ícono del archivo adjunto. |
| [getBytes()](#getBytes--) | Obtiene los datos binarios de un archivo incrustado. |
| [getExtension()](#getExtension--) | Obtiene la extensión de un archivo incrustado. |
| [getFileName()](#getFileName--) | Obtiene el nombre del archivo incrustado. |
| [getFilePath()](#getFilePath--) | Obtiene la ruta al archivo original. |
| [getHeight()](#getHeight--) | Obtiene la altura original del ícono del archivo incrustado. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtiene el desplazamiento horizontal. |
| [getIcon()](#getIcon--) | Obtiene los datos binarios del ícono asociado al archivo incrustado. |
| [getIconExtension()](#getIconExtension--) | Obtiene la extensión del ícono. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene la hora de la última modificación. |
| [getMaxHeight()](#getMaxHeight--) | Obtiene la altura máxima para mostrar el ícono del archivo incrustado. |
| [getMaxWidth()](#getMaxWidth--) | Obtiene el ancho máximo para mostrar el ícono del archivo incrustado. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Obtiene los datos del error que ocurrió al acceder al archivo. |
| [getTags()](#getTags--) | Obtiene la lista de etiquetas de un archivo adjunto. |
| [getText()](#getText--) | Obtiene la representación textual del archivo incrustado. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtiene el desplazamiento vertical. |
| [getWidth()](#getWidth--) | Obtiene el ancho original del ícono del archivo incrustado. |
| [isPrintout()](#isPrintout--) | Obtiene un valor que indica si la vista del archivo es una impresión. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Obtiene un valor que indica si el tamaño del ícono fue actualizado explícitamente por el usuario. |
| [setAlignment(int value)](#setAlignment-int-) | Establece la alineación. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Obtiene o establece un cuerpo de texto alternativo para el ícono del archivo adjunto. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Obtiene o establece un título de texto alternativo para el ícono del archivo adjunto. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Establece el desplazamiento horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Establece la hora de última modificación. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Establece la altura máxima para mostrar el ícono del archivo incrustado. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Establece el ancho máximo para mostrar el ícono del archivo incrustado. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Establece un valor que indica si la vista del archivo es una impresión. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Establece un valor que indica si el tamaño del ícono fue actualizado explícitamente por el usuario. |
| [setText(String value)](#setText-java.lang.String-) | Establece la representación textual del archivo incrustado. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Establece el desplazamiento vertical. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Inicializa una nueva instancia de la clase `AttachedFile`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | Una cadena que contiene la ruta al archivo desde el cual crear el `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Inicializa una nueva instancia de la clase `AttachedFile`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | Una cadena que contiene la ruta al archivo desde el cual crear el `AttachedFile`. |
| icono | java.io.InputStream | Un ícono para el archivo adjunto. |
| formatoIcono | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Inicializa una nueva instancia de la clase `AttachedFile`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | Un nombre del archivo adjunto. |
| attachedFileStream | java.io.InputStream | Un flujo que contiene los bytes del archivo adjunto. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Inicializa una nueva instancia de la clase `AttachedFile`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | Un nombre del archivo adjunto. |
| attachedFileStream | java.io.InputStream | Un flujo que contiene los bytes del archivo adjunto. |
| icono | java.io.InputStream | Un ícono para el archivo adjunto. |
| formatoIcono | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Un formato del ícono del archivo adjunto. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Inicializa una nueva instancia de la clase `AttachedFile`.

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


Obtiene o establece un cuerpo de texto alternativo para el ícono del archivo adjunto.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Obtiene o establece un título de texto alternativo para el ícono del archivo adjunto.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Obtiene los datos binarios de un archivo incrustado.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Obtiene la extensión de un archivo incrustado.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Obtiene el nombre del archivo incrustado.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Obtiene la ruta al archivo original.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Obtiene la altura original del ícono del archivo incrustado.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Obtiene el desplazamiento horizontal.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Obtiene los datos binarios del ícono asociado al archivo incrustado.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Obtiene la extensión del ícono.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene la hora de la última modificación.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Obtiene la altura máxima para mostrar el ícono del archivo incrustado.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Obtiene el ancho máximo para mostrar el ícono del archivo incrustado.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Obtiene los datos del error que ocurrió al acceder al archivo.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtiene la lista de etiquetas de un archivo adjunto.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Obtiene la representación de texto del archivo incrustado. La cadena NO DEBE contener ningún carácter con el valor 10 (salto de línea) o 13 (retorno de carro).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Obtiene el desplazamiento vertical.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Obtiene el ancho original del ícono del archivo incrustado.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Obtiene un valor que indica si la vista del archivo es una impresión.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Obtiene un valor que indica si el tamaño del ícono fue actualizado explícitamente por el usuario.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Establece la alineación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | Valor de Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Obtiene o establece un cuerpo de texto alternativo para el ícono del archivo adjunto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Obtiene o establece un título de texto alternativo para el ícono del archivo adjunto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Establece el desplazamiento horizontal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | Valor de Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Establece la hora de última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | Valor de Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Establece la altura máxima para mostrar el ícono del archivo incrustado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | Valor de la altura máxima. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Establece el ancho máximo para mostrar el ícono del archivo incrustado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | Valor de la anchura máxima. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Establece un valor que indica si la vista del archivo es una impresión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | Nuevo valor. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Establece un valor que indica si el tamaño del ícono fue actualizado explícitamente por el usuario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | Nuevo valor. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece la representación de texto del archivo incrustado. La cadena NO DEBE contener ningún carácter con el valor 10 (salto de línea) o 13 (retorno de carro).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | Valor de Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Establece el desplazamiento vertical.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | Valor de Offset. |

