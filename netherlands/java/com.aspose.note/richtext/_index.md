---
title: "RichText"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een rich text voor."
type: docs
weight: 82
url: /nl/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Stelt een rich text voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [RichText()](#RichText--) | Initialiseert een nieuw exemplaar van de [RichText](../../com.aspose.note/richtext)-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [append(String value)](#append-java.lang.String-) | Voegt een tekenreeks toe aan het laatste tekstbereik. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Voegt een tekenreeks toe aan het einde. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Voegt een tekenreeks toe aan het begin van het eerste tekstbereik. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Voegt een tekenreeks toe aan het begin. |
| [clear()](#clear--) | Wis de inhoud van deze instantie. |
| [getAlignment()](#getAlignment--) | Haalt de uitlijning op. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt de laatst gewijzigde tijd op. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Haalt de regelafstand op. |
| [getParagraphStyle()](#getParagraphStyle--) | Haalt de alinea-stijl op. |
| [getSpaceAfter()](#getSpaceAfter--) | Haalt de minimale hoeveelheid ruimte erna op. |
| [getSpaceBefore()](#getSpaceBefore--) | Haalt de minimale hoeveelheid ruimte ervoor op. |
| [getStyles()](#getStyles--) | Haalt de stijlen op. |
| [getTags()](#getTags--) | Haalt de lijst met alle tags van een alinea op. |
| [getText()](#getText--) | Haalt de tekst op. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Retourneert de nulgebaseerde index van de eerste voorkoming van het opgegeven Unicode‑teken in deze tekenreeks. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Retourneert de nulgebaseerde index van de eerste voorkoming van het opgegeven Unicode‑teken in deze tekenreeks. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Retourneert de nulgebaseerde index van de eerste voorkoming van het opgegeven teken in deze instantie. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in deze instantie. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in deze instantie. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in deze instantie. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in de huidige instantie. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in de huidige instantie. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in de huidige instantie. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Voegt een opgegeven tekenreeks in op een opgegeven indexpositie in deze instantie. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Voegt een opgegeven tekenreeks met opgegeven stijl in op een opgegeven indexpositie in deze instantie. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Verwijdert alle tekens in de huidige instantie, beginnend op een opgegeven positie en doorgaan tot de laatste positie. |
| [remove(int startIndex, int count)](#remove-int-int-) | Verwijdert een opgegeven aantal tekens in de huidige instantie beginnend op een opgegeven positie. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Vervangt alle voorkomens van een opgegeven Unicode‑teken in deze instantie door een ander opgegeven Unicode‑teken. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Vervangt alle voorkomens van een opgegeven tekenreeks in de huidige instantie door een andere opgegeven tekenreeks. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Vervangt alle voorkomens van een opgegeven tekenreeks in de huidige instantie door een andere opgegeven tekenreeks in opgegeven stijl. |
| [setAlignment(int value)](#setAlignment-int-) | Stelt de uitlijning in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Stelt de laatst gewijzigde tijd in. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Stelt de regelafstand in. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Stelt de alinea‑stijl in. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Stelt de minimale hoeveelheid ruimte erna in. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Stelt de minimale hoeveelheid ruimte vóór in. |
| [setText(String value)](#setText-java.lang.String-) | Stelt de tekst in. |
| [trim()](#trim--) | Verwijdert alle leidende en volgende witruimtetekens. |
| [trim(char trimChar)](#trim-char-) | Verwijdert alle leidende en volgende instanties van een teken. |
| [trim(char[] trimChars)](#trim-char...-) | Verwijdert alle leidende en volgende voorkomens van een reeks tekens die in een array zijn gespecificeerd. |
| [trimEnd()](#trimEnd--) | Verwijdert alle volgende witruimtetekens. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Verwijdert alle volgende voorkomens van een teken. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Verwijdert alle volgende voorkomens van een reeks tekens die in een array zijn gespecificeerd. |
| [trimStart()](#trimStart--) | Verwijdert alle leidende witruimtetekens. |
| [trimStart(char trimChar)](#trimStart-char-) | Verwijdert alle leidende voorkomens van een gespecificeerd teken. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Verwijdert alle leidende voorkomens van een reeks tekens die in een array zijn gespecificeerd. |
### RichText() {#RichText--}
```
public RichText()
```


Initialiseert een nieuw exemplaar van de [RichText](../../com.aspose.note/richtext)-klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse afgeleid van de [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Voegt een tekenreeks toe aan het laatste tekstbereik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De toegevoegde waarde. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Voegt een tekenreeks toe aan het einde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De toegevoegde waarde. |
| style | [TextStyle](../../com.aspose.note/textstyle) | De stijl van de toegevoegde tekenreeks. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Voegt een tekenreeks toe aan het begin van het eerste tekstbereik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De toegevoegde waarde. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Voegt een tekenreeks toe aan het begin.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De toegevoegde waarde. |
| style | [TextStyle](../../com.aspose.note/textstyle) | De stijl van de toegevoegde tekenreeks. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Wis de inhoud van deze instantie.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Haalt de uitlijning op.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt de laatst gewijzigde tijd op.

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


Haalt de regelafstand op.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Haalt de alinea-stijl op. Deze instellingen worden gebruikt als er geen overeenkomend TextStyle-object in de [getStyles](../../com.aspose.note/richtext\#getStyles) collectie is, of dit object geen benodigde instelling specificeert.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Haalt de minimale hoeveelheid ruimte erna op.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Haalt de minimale hoeveelheid ruimte ervoor op.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Haalt de stijlen op.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Haalt de lijst met alle tags van een alinea op.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Haalt de tekst op. De tekenreeks MAG GEEN tekens bevatten met de waarde 10 (regelvoeding).

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


Retourneert de nulgebaseerde index van de eerste voorkoming van het opgegeven Unicode‑teken in deze tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char | De waarde. |

**Returns:**
int - De `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Retourneert de nul-gebaseerde index van de eerste voorkoming van het opgegeven Unicode-teken in deze tekenreeks. De zoekopdracht begint op een opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char | De waarde. |
| startIndex | int | De startpositie van de zoekopdracht |

**Returns:**
int - De `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Retourneert de nul-gebaseerde index van de eerste voorkoming van het opgegeven teken in deze instantie. De zoekopdracht begint op een opgegeven tekenpositie en onderzoekt een opgegeven aantal tekenposities.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | char | De waarde. |
| startIndex | int | De startpositie van de zoekopdracht |
| count | int | Het aantal. |

**Returns:**
int - De `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in deze instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De waarde. |

**Returns:**
int - De `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Geeft de nulgebaseerde index van de eerste voorkomen van de opgegeven tekenreeks in deze instantie terug. De zoekopdracht begint op een opgegeven tekenpositie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De waarde. |
| startIndex | int | De startpositie van de zoekopdracht |

**Returns:**
int - De `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Geeft de nulgebaseerde index van de eerste voorkomen van de opgegeven tekenreeks in deze instantie terug. De zoekopdracht begint op een opgegeven tekenpositie en onderzoekt een opgegeven aantal tekenposities.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De waarde. |
| startIndex | int | De startpositie van de zoekopdracht |
| count | int | Het aantal. |

**Returns:**
int - De `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Retourneert de nulgebaseerde index van de eerste voorkoming van de opgegeven tekenreeks in de huidige instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De waarde. |
| startIndex | int | De startpositie van de zoekopdracht |
| count | int | Het aantal. |
| comparisonType | short | Het type zoekopdracht dat moet worden gebruikt voor de opgegeven tekenreeks |

**Returns:**
int - De `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Geeft de nulgebaseerde index van de eerste voorkomen van de opgegeven tekenreeks in de huidige instantie terug. Een parameter specificeert het type zoekopdracht dat moet worden gebruikt voor de opgegeven tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De waarde. |
| comparisonType | short | Het type zoekopdracht dat moet worden gebruikt voor de opgegeven tekenreeks |

**Returns:**
int - De `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Geeft de nulgebaseerde index van de eerste voorkomen van de opgegeven tekenreeks in de huidige instantie terug. Parameters geven de startzoekpositie in de huidige tekenreeks en het type zoekopdracht dat moet worden gebruikt voor de opgegeven tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | De waarde. |
| startIndex | int | De startpositie van de zoekopdracht |
| comparisonType | short | Het type zoekopdracht dat moet worden gebruikt voor de opgegeven tekenreeks |

**Returns:**
int - De `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Voegt een opgegeven tekenreeks in op een opgegeven indexpositie in deze instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| startIndex | int | De startindex. |
| waarde | java.lang.String | De waarde. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Voegt een opgegeven tekenreeks met opgegeven stijl in op een opgegeven indexpositie in deze instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| startIndex | int | De startindex. |
| waarde | java.lang.String | De waarde. |
| style | [TextStyle](../../com.aspose.note/textstyle) | De stijl. |

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


Verwijdert alle tekens in de huidige instantie, beginnend op een opgegeven positie en doorgaan tot de laatste positie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| startIndex | int | De startindex. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Verwijdert een opgegeven aantal tekens in de huidige instantie beginnend op een opgegeven positie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| startIndex | int | De startindex. |
| count | int | Het aantal. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Vervangt alle voorkomens van een opgegeven Unicode‑teken in deze instantie door een ander opgegeven Unicode‑teken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldChar | char | Het oude teken. |
| newChar | char | Het nieuwe teken. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Vervangt alle voorkomens van een opgegeven tekenreeks in de huidige instantie door een andere opgegeven tekenreeks.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | java.lang.String | De oude waarde. |
| newValue | java.lang.String | De nieuwe waarde. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Vervangt alle voorkomens van een opgegeven tekenreeks in de huidige instantie door een andere opgegeven tekenreeks in opgegeven stijl.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldValue | java.lang.String | De oude waarde. |
| newValue | java.lang.String | De nieuwe waarde. |
| style | [TextStyle](../../com.aspose.note/textstyle) | De stijl van de nieuwe waarde. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Stelt de uitlijning in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Stelt de regelafstand in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Stelt de alinea‑stijl in. Deze instellingen worden gebruikt als er geen overeenkomend TextStyle‑object in de [getStyles](../../com.aspose.note/richtext\#getStyles)‑collectie bestaat of dit object geen benodigde instelling opgeeft.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Stelt de minimale hoeveelheid ruimte erna in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Stelt de minimale hoeveelheid ruimte vóór in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Stelt de tekst in. De tekenreeks MAG GEEN tekens met de waarde 10 (regelvoeding) bevatten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Verwijdert alle leidende en volgende witruimtetekens.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Verwijdert alle leidende en volgende instanties van een teken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trimChar | char | Het trimteken. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Verwijdert alle leidende en volgende voorkomens van een reeks tekens die in een array zijn gespecificeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trimChars | char[] | De trimtekens. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Verwijdert alle volgende witruimtetekens.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Verwijdert alle volgende voorkomens van een teken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trimChar | char | Het trimteken. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Verwijdert alle volgende voorkomens van een reeks tekens die in een array zijn gespecificeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trimChars | char[] | De trimtekens. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Verwijdert alle leidende witruimtetekens.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Verwijdert alle leidende voorkomens van een gespecificeerd teken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trimChar | char | Het trimteken. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Verwijdert alle leidende voorkomens van een reeks tekens die in een array zijn gespecificeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| trimChars | char[] | De trimtekens. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
