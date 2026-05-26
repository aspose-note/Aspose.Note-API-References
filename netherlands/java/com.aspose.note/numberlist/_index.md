---
title: "NumberList"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt de genummerde of opsomminglijst voor."
type: docs
weight: 64
url: /nl/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Stelt de genummerde of opsomminglijst voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Initialiseert een nieuw exemplaar van de `NumberList`-klasse. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Initialiseert een nieuw exemplaar van de `NumberList`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [getFont()](#getFont--) | Haalt de naam van het lettertype op of stelt deze in. |
| [getFontColor()](#getFontColor--) | Haalt de letterkleur op of stelt deze in. |
| [getFontSize()](#getFontSize--) | Haalt de lettergrootte op of stelt deze in. |
| [getFormat()](#getFormat--) | Haalt het formaat van de regelkop op of stelt dit in. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getNumberFormat()](#getNumberFormat--) | Haalt het getalformaat op dat wordt gebruikt voor een groep automatisch genummerde objecten, of stelt dit in. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Haalt de genummerde lijstkop op. |
| [getRestart()](#getRestart--) | Haalt de numerieke waarde op die de automatische nummerwaarde van het lijstitem overschrijft, of stelt deze in. |
| [hashCode()](#hashCode--) | Dient als een hash-functie voor het type. |
| [isBold()](#isBold--) | Haalt een waarde op of stelt deze in die aangeeft of de tekststijl vetgedrukt is. |
| [isItalic()](#isItalic--) | Haalt een waarde op of stelt deze in die aangeeft of de tekststijl cursief is. |
| [setBold(boolean value)](#setBold-boolean-) | Haalt een waarde op of stelt deze in die aangeeft of de tekststijl vetgedrukt is. |
| [setFont(String value)](#setFont-java.lang.String-) | Haalt de naam van het lettertype op of stelt deze in. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Haalt de letterkleur op of stelt deze in. |
| [setFontSize(int value)](#setFontSize-int-) | Haalt de lettergrootte op of stelt deze in. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Haalt het formaat van de regelkop op of stelt dit in. |
| [setItalic(boolean value)](#setItalic-boolean-) | Haalt een waarde op of stelt deze in die aangeeft of de tekststijl cursief is. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Haalt het getalformaat op dat wordt gebruikt voor een groep automatisch genummerde objecten, of stelt dit in. |
| [setRestart(int value)](#setRestart-int-) | Haalt de numerieke waarde op die de automatische nummerwaarde van het lijstitem overschrijft, of stelt deze in. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Initialiseert een nieuw exemplaar van de `NumberList`-klasse. Deze instantie vertegenwoordigt een opsomming met opsommingstekens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Een symbool dat een opsommingsteken vertegenwoordigt. |
| font | java.lang.String | Een lettertype voor het opsommingsteken. |
| fontSize | int | Een lettergrootte voor het opsommingsteken. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Initialiseert een nieuw exemplaar van de `NumberList`-klasse. Deze instantie vertegenwoordigt een genummerde lijst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| format | java.lang.String | Het formaat van de genummerde kop. |
| numberFormat | byte | Het formaat van het nummer in de koptekst. |
| font | java.lang.String | Een lettertype voor de genummerde koptekst. |
| fontSize | int | Een lettergrootte voor de genummerde koptekst. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Bepaalt of het opgegeven object gelijk is aan het huidige object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Het object. |

**Returns:**
boolean - De `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bepaalt of het opgegeven object gelijk is aan het huidige object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object. |

**Returns:**
boolean - De `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Haalt de naam van het lettertype op of stelt deze in.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Haalt de letterkleur op of stelt deze in.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Haalt de lettergrootte op of stelt deze in.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Haalt het formaat van de regelkop op of stelt het in. Voor opsommingslijsten vertegenwoordigt het een opsommingsteken.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Haalt het getalformaat op dat wordt gebruikt voor een groep automatisch genummerde objecten, of stelt het in. Moet null zijn voor opsommingslijsten.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Haalt de genummerde lijstkop op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sequenceNumber | int | Het volgnummer in de genummerde lijst. |

**Returns:**
java.lang.String - Een tekenreeksrepresentatie van het opgegeven volgnummer.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Haalt de numerieke waarde op die de automatische nummerwaarde van het lijstitem overschrijft, of stelt deze in.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als een hash-functie voor het type.

**Returns:**
int - De `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Haalt een waarde op of stelt deze in die aangeeft of de tekststijl vetgedrukt is.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Haalt een waarde op of stelt deze in die aangeeft of de tekststijl cursief is.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Haalt een waarde op of stelt deze in die aangeeft of de tekststijl vetgedrukt is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Haalt de naam van het lettertype op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Haalt de letterkleur op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Haalt de lettergrootte op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Haalt het formaat van de regelkop op of stelt het in. Voor opsommingslijsten vertegenwoordigt het een opsommingsteken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Haalt een waarde op of stelt deze in die aangeeft of de tekststijl cursief is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Haalt het getalformaat op dat wordt gebruikt voor een groep automatisch genummerde objecten, of stelt het in. Moet null zijn voor opsommingslijsten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Haalt de numerieke waarde op die de automatische nummerwaarde van het lijstitem overschrijft, of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

