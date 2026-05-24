---
title: "NumberList"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente la liste numérotée ou à puces."
type: docs
weight: 64
url: /fr/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Représente la liste numérotée ou à puces.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Initialise une nouvelle instance de la classe `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Initialise une nouvelle instance de la classe `NumberList`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [getFont()](#getFont--) | Obtient ou définit le nom de la police. |
| [getFontColor()](#getFontColor--) | Obtient ou définit la couleur de la police. |
| [getFontSize()](#getFontSize--) | Obtient ou définit la taille de la police. |
| [getFormat()](#getFormat--) | Obtient ou définit le format de l'en-tête de ligne. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getNumberFormat()](#getNumberFormat--) | Obtient ou définit le format numérique utilisé pour un groupe d'objets numérotés automatiquement. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Obtient l'en-tête de la liste numérotée. |
| [getRestart()](#getRestart--) | Obtient ou définit la valeur numérique qui remplace la valeur de numéro automatique de l'élément de liste. |
| [hashCode()](#hashCode--) | Servit de fonction de hachage pour le type. |
| [isBold()](#isBold--) | Obtient ou définit une valeur indiquant si le style de texte est en gras. |
| [isItalic()](#isItalic--) | Obtient ou définit une valeur indiquant si le style de texte est en italique. |
| [setBold(boolean value)](#setBold-boolean-) | Obtient ou définit une valeur indiquant si le style de texte est en gras. |
| [setFont(String value)](#setFont-java.lang.String-) | Obtient ou définit le nom de la police. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Obtient ou définit la couleur de la police. |
| [setFontSize(int value)](#setFontSize-int-) | Obtient ou définit la taille de la police. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Obtient ou définit le format de l'en-tête de ligne. |
| [setItalic(boolean value)](#setItalic-boolean-) | Obtient ou définit une valeur indiquant si le style de texte est en italique. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Obtient ou définit le format numérique utilisé pour un groupe d'objets numérotés automatiquement. |
| [setRestart(int value)](#setRestart-int-) | Obtient ou définit la valeur numérique qui remplace la valeur de numéro automatique de l'élément de liste. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Initialise une nouvelle instance de la classe `NumberList`. Cette instance représente une liste à puces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Un symbole qui représente une puce. |
| police | java.lang.String | Une police pour la puce. |
| fontSize | int | Une taille de police pour la puce. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Initialise une nouvelle instance de la classe `NumberList`. Cette instance représente une liste numérotée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| format | java.lang.String | Le format de l'en-tête numéroté. |
| numberFormat | byte | Le format du numéro dans l'en-tête. |
| police | java.lang.String | Une police pour l'en-tête numéroté. |
| fontSize | int | Une taille de police pour l'en-tête numéroté. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Détermine si l'objet spécifié est égal à l'objet actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | L'objet. |

**Returns:**
booléen - Le `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si l'objet spécifié est égal à l'objet actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet. |

**Returns:**
booléen - Le `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Obtient ou définit le nom de la police.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Obtient ou définit la couleur de la police.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Obtient ou définit la taille de la police.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Obtient ou définit le format de l'en-tête de ligne. Pour les listes à puces, représente un symbole de puce.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient ou définit l'heure de la dernière modification.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Obtient ou définit le format de numéro utilisé pour un groupe d'objets numérotés automatiquement. Doit être nul pour les listes à puces.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Obtient l'en-tête de la liste numérotée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sequenceNumber | int | Le numéro de séquence dans la liste numérotée. |

**Returns:**
java.lang.String - Une représentation sous forme de chaîne du numéro de séquence spécifié.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Obtient ou définit la valeur numérique qui remplace la valeur de numéro automatique de l'élément de liste.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Servit de fonction de hachage pour le type.

**Returns:**
int - Le `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Obtient ou définit une valeur indiquant si le style de texte est en gras.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtient ou définit une valeur indiquant si le style de texte est en italique.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Obtient ou définit une valeur indiquant si le style de texte est en gras.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Obtient ou définit le nom de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Obtient ou définit la couleur de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Obtient ou définit la taille de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Obtient ou définit le format de l'en-tête de ligne. Pour les listes à puces, représente un symbole de puce.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Obtient ou définit une valeur indiquant si le style de texte est en italique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Obtient ou définit le format de numéro utilisé pour un groupe d'objets numérotés automatiquement. Doit être nul pour les listes à puces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Obtient ou définit la valeur numérique qui remplace la valeur de numéro automatique de l'élément de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

