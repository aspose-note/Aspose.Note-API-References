---
title: "NumberList"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar den numrerade eller punktlistan."
type: docs
weight: 64
url: /sv/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Representerar den numrerade eller punktlistan.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Initierar en ny instans av klassen `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Initierar en ny instans av klassen `NumberList`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| [getFont()](#getFont--) | Hämtar eller anger namnet på teckensnittet. |
| [getFontColor()](#getFontColor--) | Hämtar eller anger teckensnittsfärgen. |
| [getFontSize()](#getFontSize--) | Hämtar eller anger teckensnittsstorleken. |
| [getFormat()](#getFormat--) | Hämtar eller anger formatet för radhuvudet. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar eller anger den senast ändrade tiden. |
| [getNumberFormat()](#getNumberFormat--) | Hämtar eller anger talformatet som används för en grupp av automatiskt numrerade objekt. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Hämtar rubriken för den numrerade listan. |
| [getRestart()](#getRestart--) | Hämtar eller anger det numeriska värdet som åsidosätter det automatiska nummervärdet för listobjektet. |
| [hashCode()](#hashCode--) | Fungerar som en hash-funktion för typen. |
| [isBold()](#isBold--) | Hämtar eller anger ett värde som indikerar om textstilen är fet. |
| [isItalic()](#isItalic--) | Hämtar eller anger ett värde som indikerar om textstilen är kursiv. |
| [setBold(boolean value)](#setBold-boolean-) | Hämtar eller anger ett värde som indikerar om textstilen är fet. |
| [setFont(String value)](#setFont-java.lang.String-) | Hämtar eller anger namnet på teckensnittet. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Hämtar eller anger teckensnittsfärgen. |
| [setFontSize(int value)](#setFontSize-int-) | Hämtar eller anger teckensnittsstorleken. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Hämtar eller anger formatet för radhuvudet. |
| [setItalic(boolean value)](#setItalic-boolean-) | Hämtar eller anger ett värde som indikerar om textstilen är kursiv. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Hämtar eller anger den senast ändrade tiden. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Hämtar eller anger talformatet som används för en grupp av automatiskt numrerade objekt. |
| [setRestart(int value)](#setRestart-int-) | Hämtar eller anger det numeriska värdet som åsidosätter det automatiska nummervärdet för listobjektet. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Initierar en ny instans av klassen `NumberList`. Denna instans representerar en punktlista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | En symbol som representerar ett punkttecken. |
| font | java.lang.String | Ett teckensnitt för punkttecknet. |
| fontSize | int | En teckensnittsstorlek för punkttecknet. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Initierar en ny instans av klassen `NumberList`. Denna instans representerar en numrerad lista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | java.lang.String | Formatet för den numrerade rubriken. |
| numberFormat | byte | Formatet för numret i rubriken. |
| font | java.lang.String | Ett teckensnitt för den numrerade rubriken. |
| fontSize | int | En teckenstorlek för den numrerade rubriken. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Bestämmer om det angivna objektet är lika med det aktuella objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Objektet. |

**Returns:**
boolean - `bool`-typen.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestämmer om det angivna objektet är lika med det aktuella objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet. |

**Returns:**
boolean - `bool`-typen.
### getFont() {#getFont--}
```
public String getFont()
```


Hämtar eller anger namnet på teckensnittet.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Hämtar eller anger teckensnittsfärgen.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Hämtar eller anger teckensnittsstorleken.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Hämtar eller anger formatet för radrubriken. För punktlistor representerar den en punktsymbol.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar eller anger den senast ändrade tiden.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Hämtar eller anger talformatet som används för en grupp av automatiskt numrerade objekt. Ska vara null för punktlistor.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Hämtar rubriken för den numrerade listan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sequenceNumber | int | Sekvensnumret i den numrerade listan. |

**Returns:**
java.lang.String - En strängrepresentation av det angivna sekvensnumret.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Hämtar eller anger det numeriska värdet som åsidosätter det automatiska nummervärdet för listobjektet.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Fungerar som en hash-funktion för typen.

**Returns:**
int - `int`-typen.
### isBold() {#isBold--}
```
public boolean isBold()
```


Hämtar eller anger ett värde som indikerar om textstilen är fet.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Hämtar eller anger ett värde som indikerar om textstilen är kursiv.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Hämtar eller anger ett värde som indikerar om textstilen är fet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Hämtar eller anger namnet på teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Hämtar eller anger teckensnittsfärgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Hämtar eller anger teckensnittsstorleken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Hämtar eller anger formatet för radrubriken. För punktlistor representerar den en punktsymbol.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Hämtar eller anger ett värde som indikerar om textstilen är kursiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Hämtar eller anger den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Hämtar eller anger talformatet som används för en grupp av automatiskt numrerade objekt. Ska vara null för punktlistor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Hämtar eller anger det numeriska värdet som åsidosätter det automatiska nummervärdet för listobjektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

