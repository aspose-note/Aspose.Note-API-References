---
title: "NumberList"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa la lista numerada o con viñetas."
type: docs
weight: 64
url: /es/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Representa la lista numerada o con viñetas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Inicializa una nueva instancia de la clase `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Inicializa una nueva instancia de la clase `NumberList`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Determina si el objeto especificado es igual al objeto actual. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si el objeto especificado es igual al objeto actual. |
| [getFont()](#getFont--) | Obtiene o establece el nombre de la fuente. |
| [getFontColor()](#getFontColor--) | Obtiene o establece el color de la fuente. |
| [getFontSize()](#getFontSize--) | Obtiene o establece el tamaño de la fuente. |
| [getFormat()](#getFormat--) | Obtiene o establece el formato del encabezado de línea. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene o establece la hora de la última modificación. |
| [getNumberFormat()](#getNumberFormat--) | Obtiene o establece el formato numérico usado para un grupo de objetos numerados automáticamente. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Obtiene el encabezado de la lista numerada. |
| [getRestart()](#getRestart--) | Obtiene o establece el valor numérico que sobrescribe el valor automático del número del elemento de la lista. |
| [hashCode()](#hashCode--) | Funciona como una función hash para el tipo. |
| [isBold()](#isBold--) | Obtiene o establece un valor que indica si el estilo de texto es negrita. |
| [isItalic()](#isItalic--) | Obtiene o establece un valor que indica si el estilo de texto es cursiva. |
| [setBold(boolean value)](#setBold-boolean-) | Obtiene o establece un valor que indica si el estilo de texto es negrita. |
| [setFont(String value)](#setFont-java.lang.String-) | Obtiene o establece el nombre de la fuente. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Obtiene o establece el color de la fuente. |
| [setFontSize(int value)](#setFontSize-int-) | Obtiene o establece el tamaño de la fuente. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Obtiene o establece el formato del encabezado de línea. |
| [setItalic(boolean value)](#setItalic-boolean-) | Obtiene o establece un valor que indica si el estilo de texto es cursiva. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtiene o establece la hora de la última modificación. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Obtiene o establece el formato numérico usado para un grupo de objetos numerados automáticamente. |
| [setRestart(int value)](#setRestart-int-) | Obtiene o establece el valor numérico que sobrescribe el valor automático del número del elemento de la lista. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Inicializa una nueva instancia de la clase `NumberList`. Esta instancia representa una lista con viñetas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Un símbolo que representa una viñeta. |
| fuente | java.lang.String | Una fuente para la viñeta. |
| fontSize | int | Un tamaño de fuente para la viñeta. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Inicializa una nueva instancia de la clase `NumberList`. Esta instancia representa una lista numerada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| format | java.lang.String | El formato del encabezado numerado. |
| numberFormat | byte | El formato del número en el encabezado. |
| fuente | java.lang.String | Una fuente para el encabezado numerado. |
| fontSize | int | Un tamaño de fuente para el encabezado numerado. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Determina si el objeto especificado es igual al objeto actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | El objeto. |

**Returns:**
boolean - El `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si el objeto especificado es igual al objeto actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto. |

**Returns:**
boolean - El `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Obtiene o establece el nombre de la fuente.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Obtiene o establece el color de la fuente.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Obtiene o establece el tamaño de la fuente.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Obtiene o establece el formato del encabezado de línea. Para listas con viñetas representa un símbolo de viñeta.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene o establece la hora de la última modificación.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Obtiene o establece el formato numérico utilizado para un grupo de objetos numerados automáticamente. Debe ser nulo para listas con viñetas.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Obtiene el encabezado de la lista numerada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sequenceNumber | int | El número de secuencia en la lista numerada. |

**Returns:**
java.lang.String - Una representación en cadena del número de secuencia especificado.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Obtiene o establece el valor numérico que sobrescribe el valor automático del número del elemento de la lista.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funciona como una función hash para el tipo.

**Returns:**
int - El `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Obtiene o establece un valor que indica si el estilo de texto es negrita.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtiene o establece un valor que indica si el estilo de texto es cursiva.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Obtiene o establece un valor que indica si el estilo de texto es negrita.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Obtiene o establece el nombre de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Obtiene o establece el color de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Obtiene o establece el tamaño de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Obtiene o establece el formato del encabezado de línea. Para listas con viñetas representa un símbolo de viñeta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Obtiene o establece un valor que indica si el estilo de texto es cursiva.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtiene o establece la hora de la última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Obtiene o establece el formato numérico utilizado para un grupo de objetos numerados automáticamente. Debe ser nulo para listas con viñetas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Obtiene o establece el valor numérico que sobrescribe el valor automático del número del elemento de la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

