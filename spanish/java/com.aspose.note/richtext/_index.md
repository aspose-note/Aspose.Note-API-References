---
title: "RichText"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un texto enriquecido."
type: docs
weight: 82
url: /es/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Representa un texto enriquecido.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RichText()](#RichText--) | Inicializa una nueva instancia de la clase [RichText](../../com.aspose.note/richtext). |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [append(String value)](#append-java.lang.String-) | Agrega una cadena al último rango de texto. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Agrega una cadena al final. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Agrega una cadena al principio del primer rango de texto. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Agrega una cadena al principio. |
| [clear()](#clear--) | Borra el contenido de esta instancia. |
| [getAlignment()](#getAlignment--) | Obtiene la alineación. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene la hora de la última modificación. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Obtiene el interlineado. |
| [getParagraphStyle()](#getParagraphStyle--) | Obtiene el estilo del párrafo. |
| [getSpaceAfter()](#getSpaceAfter--) | Obtiene la cantidad mínima de espacio después. |
| [getSpaceBefore()](#getSpaceBefore--) | Obtiene la cantidad mínima de espacio antes. |
| [getStyles()](#getStyles--) | Obtiene los estilos. |
| [getTags()](#getTags--) | Obtiene la lista de todas las etiquetas de un párrafo. |
| [getText()](#getText--) | Obtiene el texto. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Devuelve el índice basado en cero de la primera aparición del carácter Unicode especificado en esta cadena. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Devuelve el índice basado en cero de la primera aparición del carácter Unicode especificado en esta cadena. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Devuelve el índice basado en cero de la primera aparición del carácter especificado en esta instancia. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Devuelve el índice basado en cero de la primera aparición de la cadena especificada en esta instancia. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Devuelve el índice basado en cero de la primera aparición de la cadena especificada en esta instancia. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Devuelve el índice basado en cero de la primera aparición de la cadena especificada en esta instancia. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Devuelve el índice basado en cero de la primera aparición de la cadena especificada en la instancia actual. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Devuelve el índice basado en cero de la primera aparición de la cadena especificada en la instancia actual. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Devuelve el índice basado en cero de la primera aparición de la cadena especificada en la instancia actual. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Inserta una cadena especificada en una posición de índice especificada en esta instancia. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Inserta una cadena especificada con estilo especificado en una posición de índice especificada en esta instancia. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Elimina todos los caracteres en la instancia actual, comenzando en una posición especificada y continuando hasta la última posición. |
| [remove(int startIndex, int count)](#remove-int-int-) | Elimina el número especificado de caracteres en la instancia actual comenzando en una posición especificada. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Reemplaza todas las apariciones de un carácter Unicode especificado en esta instancia con otro carácter Unicode especificado. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Reemplaza todas las apariciones de una cadena especificada en la instancia actual con otra cadena especificada. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Reemplaza todas las apariciones de una cadena especificada en la instancia actual con otra cadena especificada en el estilo especificado. |
| [setAlignment(int value)](#setAlignment-int-) | Establece la alineación. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Establece la hora de última modificación. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Establece el interlineado. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Establece el estilo del párrafo. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Establece la cantidad mínima de espacio después. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Establece la cantidad mínima de espacio antes. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto. |
| [trim()](#trim--) | Elimina todos los caracteres de espacio en blanco al principio y al final. |
| [trim(char trimChar)](#trim-char-) | Elimina todas las instancias de un carácter al principio y al final. |
| [trim(char[] trimChars)](#trim-char...-) | Elimina todas las ocurrencias al principio y al final de un conjunto de caracteres especificado en una matriz. |
| [trimEnd()](#trimEnd--) | Elimina todos los caracteres de espacio en blanco al final. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Elimina todas las ocurrencias al final de un carácter. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Elimina todas las ocurrencias al final de un conjunto de caracteres especificado en una matriz. |
| [trimStart()](#trimStart--) | Elimina todos los caracteres de espacio en blanco al principio. |
| [trimStart(char trimChar)](#trimStart-char-) | Elimina todas las ocurrencias al principio de un carácter especificado. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Elimina todas las ocurrencias al principio de un conjunto de caracteres especificado en una matriz. |
### RichText() {#RichText--}
```
public RichText()
```


Inicializa una nueva instancia de la clase [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Agrega una cadena al último rango de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor añadido. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Agrega una cadena al final.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor añadido. |
| style | [TextStyle](../../com.aspose.note/textstyle) | El estilo de la cadena añadida. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Agrega una cadena al principio del primer rango de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor añadido. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Agrega una cadena al principio.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor añadido. |
| style | [TextStyle](../../com.aspose.note/textstyle) | El estilo de la cadena añadida. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Borra el contenido de esta instancia.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Obtiene la alineación.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene la hora de la última modificación.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Obtiene el interlineado.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Obtiene el estilo del párrafo. Estas configuraciones se utilizan si no hay un objeto TextStyle coincidente en la colección [getStyles](../../com.aspose.note/richtext\\#getStyles) o si este objeto no especifica la configuración necesaria.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Obtiene la cantidad mínima de espacio después.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Obtiene la cantidad mínima de espacio antes.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Obtiene los estilos.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtiene la lista de todas las etiquetas de un párrafo.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Obtiene el texto. La cadena NO DEBE contener ningún carácter con el valor 10 (salto de línea).

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Devuelve el índice basado en cero de la primera aparición del carácter Unicode especificado en esta cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char | El valor. |

**Returns:**
int - El `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Devuelve el índice basado en cero de la primera aparición del carácter Unicode especificado en esta cadena. La búsqueda comienza en una posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char | El valor. |
| startIndex | int | La posición inicial de búsqueda |

**Returns:**
int - El `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Devuelve el índice basado en cero de la primera aparición del carácter especificado en esta instancia. La búsqueda comienza en una posición de carácter especificada y examina un número especificado de posiciones de carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char | El valor. |
| startIndex | int | La posición inicial de búsqueda |
| count | int | El recuento. |

**Returns:**
int - El `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Devuelve el índice basado en cero de la primera aparición de la cadena especificada en esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor. |

**Returns:**
int - El `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Devuelve el índice basado en cero de la primera aparición de la cadena especificada en esta instancia. La búsqueda comienza en una posición de carácter especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor. |
| startIndex | int | La posición inicial de búsqueda |

**Returns:**
int - El `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Devuelve el índice basado en cero de la primera aparición de la cadena especificada en esta instancia. La búsqueda comienza en una posición de carácter especificada y examina un número especificado de posiciones de carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor. |
| startIndex | int | La posición inicial de búsqueda |
| count | int | El recuento. |

**Returns:**
int - El `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Devuelve el índice basado en cero de la primera aparición de la cadena especificada en la instancia actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor. |
| startIndex | int | La posición inicial de búsqueda |
| count | int | El recuento. |
| comparisonType | short | El tipo de búsqueda a utilizar para la cadena especificada |

**Returns:**
int - El `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Devuelve el índice basado en cero de la primera aparición de la cadena especificada en la instancia actual. Un parámetro especifica el tipo de búsqueda a utilizar para la cadena especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor. |
| comparisonType | short | El tipo de búsqueda a utilizar para la cadena especificada |

**Returns:**
int - El `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Devuelve el índice basado en cero de la primera aparición de la cadena especificada en la instancia actual. Los parámetros especifican la posición inicial de búsqueda en la cadena actual y el tipo de búsqueda a utilizar para la cadena especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor. |
| startIndex | int | La posición inicial de búsqueda |
| comparisonType | short | El tipo de búsqueda a utilizar para la cadena especificada |

**Returns:**
int - El `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Inserta una cadena especificada en una posición de índice especificada en esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |
| valor | java.lang.String | El valor. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Inserta una cadena especificada con estilo especificado en una posición de índice especificada en esta instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |
| valor | java.lang.String | El valor. |
| style | [TextStyle](../../com.aspose.note/textstyle) | El estilo. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Elimina todos los caracteres en la instancia actual, comenzando en una posición especificada y continuando hasta la última posición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Elimina el número especificado de caracteres en la instancia actual comenzando en una posición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |
| count | int | El recuento. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Reemplaza todas las apariciones de un carácter Unicode especificado en esta instancia con otro carácter Unicode especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldChar | char | El carácter antiguo. |
| newChar | char | El carácter nuevo. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Reemplaza todas las apariciones de una cadena especificada en la instancia actual con otra cadena especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldValue | java.lang.String | El valor antiguo. |
| newValue | java.lang.String | El valor nuevo. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Reemplaza todas las apariciones de una cadena especificada en la instancia actual con otra cadena especificada en el estilo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldValue | java.lang.String | El valor antiguo. |
| newValue | java.lang.String | El valor nuevo. |
| style | [TextStyle](../../com.aspose.note/textstyle) | El estilo del valor nuevo. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Establece la alineación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Establece la hora de última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Establece el interlineado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Establece el estilo del párrafo. Estas configuraciones se utilizan si no hay un objeto TextStyle coincidente en la colección [getStyles](../../com.aspose.note/richtext\#getStyles) o si este objeto no especifica una configuración necesaria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Establece la cantidad mínima de espacio después.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Establece la cantidad mínima de espacio antes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Establece el texto. La cadena NO DEBE contener ningún carácter con el valor 10 (salto de línea).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Elimina todos los caracteres de espacio en blanco al principio y al final.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Elimina todas las instancias de un carácter al principio y al final.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| trimChar | char | El carácter de recorte. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Elimina todas las ocurrencias al principio y al final de un conjunto de caracteres especificado en una matriz.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| trimChars | char[] | Los caracteres de recorte. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Elimina todos los caracteres de espacio en blanco al final.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Elimina todas las ocurrencias al final de un carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| trimChar | char | El carácter de recorte. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Elimina todas las ocurrencias al final de un conjunto de caracteres especificado en una matriz.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| trimChars | char[] | Los caracteres de recorte. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Elimina todos los caracteres de espacio en blanco al principio.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Elimina todas las ocurrencias al principio de un carácter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| trimChar | char | El carácter de recorte. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Elimina todas las ocurrencias al principio de un conjunto de caracteres especificado en una matriz.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| trimChars | char[] | Los caracteres de recorte. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
