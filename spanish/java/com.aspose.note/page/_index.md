---
title: "Page"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa una página."
type: docs
weight: 69
url: /es/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Representa una página.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Page()](#Page--) | Inicializa una nueva instancia de la clase `Page`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [deepClone()](#deepClone--) | Clona la página. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Clona la página. |
| [getAuthor()](#getAuthor--) | Obtiene o establece el autor. |
| [getBackgroundColor()](#getBackgroundColor--) | Obtiene o establece el color de fondo de la página. |
| [getCreationTime()](#getCreationTime--) | Obtiene o establece la hora de creación. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene o establece la hora de la última modificación. |
| [getLevel()](#getLevel--) | Obtiene o establece el nivel. |
| [getMargin()](#getMargin--) | Obtiene o establece el margen. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Obtiene o establece el resumen de revisión para la página y sus nodos hijos. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Obtiene el tamaño de diseño de la página mostrado en el editor. |
| [getSizeType()](#getSizeType--) | Obtiene o establece el tipo de tamaño de una página. |
| [getTitle()](#getTitle--) | Obtiene o establece el título. |
| [isConflictPage()](#isConflictPage--) | Obtiene o establece un valor que indica si esta página es una página de conflicto. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Obtiene o establece el autor. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Obtiene o establece el color de fondo de la página. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Obtiene o establece un valor que indica si esta página es una página de conflicto. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Obtiene o establece la hora de creación. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtiene o establece la hora de la última modificación. |
| [setLevel(byte value)](#setLevel-byte-) | Obtiene o establece el nivel. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Obtiene o establece el margen. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Obtiene o establece el resumen de revisión para la página y sus nodos hijos. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Establece el tamaño del diseño de la página que se muestra en el editor. |
| [setSizeType(int value)](#setSizeType-int-) | Obtiene o establece el tipo de tamaño de una página. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Obtiene o establece el título. |
### Page() {#Page--}
```
public Page()
```


Inicializa una nueva instancia de la clase `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Clona la página.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Clona la página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cloneHistory | boolean | Especifica si el historial de la página debe ser clonado.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtiene o establece el autor.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Obtiene o establece el color de fondo de la página.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Obtiene o establece la hora de creación.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene o establece la hora de la última modificación.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Obtiene o establece el nivel.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Obtiene o establece el margen.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Obtiene o establece el resumen de revisión para la página y sus nodos hijos.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Obtiene el tamaño de diseño de la página mostrado en el editor.

--------------------

Este valor es utilizado por la aplicación Microsoft OneNote para mostrar el diseño subyacente de la página cuando se abre el documento. De todos modos, no afecta la impresión ni el guardado del documento. Cuando la propiedad Page.SizeType se establece en PageSizeType.SizeByContent, esta propiedad devuelve el tamaño real del contenido.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Obtiene o establece el tipo de tamaño de una página.

--------------------

Por defecto, una página cambia de tamaño automáticamente. El valor predeterminado es [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Obtiene o establece el título.

Valor: El `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Obtiene o establece un valor que indica si esta página es una página de conflicto.

--------------------

La página de conflicto surge cuando dos usuarios intentan actualizar el mismo contenido. En este caso, los cambios del primer usuario se guardan como de costumbre. Pero los cambios del otro usuario no pueden fusionarse. Por lo tanto, solo se crea una copia de la página y se marca como conflicto.

En esta versión, los conflictos se resuelven a favor de los cambios del primer usuario. Por lo tanto, si el documento tiene páginas de conflicto, se mostrarán en el historial pero se omitirán al guardar. Es posible restablecer esta bandera para guardar estas páginas en el historial como páginas normales.

Se puede encontrar un ejemplo detallado de manipulación de páginas de conflicto en la documentación en línea.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Obtiene o establece el autor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Obtiene o establece el color de fondo de la página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Obtiene o establece un valor que indica si esta página es una página de conflicto.

--------------------

La página de conflicto surge cuando dos usuarios intentan actualizar el mismo contenido. En este caso, los cambios del primer usuario se guardan como de costumbre. Pero los cambios del otro usuario no pueden fusionarse. Por lo tanto, solo se crea una copia de la página y se marca como conflicto.

En esta versión, los conflictos se resuelven a favor de los cambios del primer usuario. Por lo tanto, si el documento tiene páginas de conflicto, se mostrarán en el historial pero se omitirán al guardar. Es posible restablecer esta bandera para guardar estas páginas en el historial como páginas normales.

Se puede encontrar un ejemplo detallado de manipulación de páginas de conflicto en la documentación en línea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Obtiene o establece la hora de creación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtiene o establece la hora de la última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Obtiene o establece el nivel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Obtiene o establece el margen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Obtiene o establece el resumen de revisión para la página y sus nodos hijos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Establece el tamaño del diseño de la página que se muestra en el editor.

--------------------

Este valor es utilizado por la aplicación Microsoft OneNote para mostrar el diseño subyacente de la página cuando se abre el documento. De todos modos, no afecta la impresión ni el guardado del documento. Cuando la propiedad Page.SizeType se establece en PageSizeType.SizeByContent, esta propiedad devuelve el tamaño real del contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Obtiene o establece el tipo de tamaño de una página.

--------------------

Por defecto, una página cambia de tamaño automáticamente. El valor predeterminado es [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Obtiene o establece el título.

Valor: El `Title`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

