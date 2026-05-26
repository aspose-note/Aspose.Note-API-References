---
title: "RichText"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en rich text."
type: docs
weight: 82
url: /sv/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Representerar en rich text.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [RichText()](#RichText--) | Initierar en ny instans av klassen [RichText](../../com.aspose.note/richtext). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [append(String value)](#append-java.lang.String-) | Lägger till en sträng i det sista textintervallet. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Lägger till en sträng i slutet. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Lägger till en sträng i början av det första textintervallet. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Lägger till en sträng i början. |
| [clear()](#clear--) | Rensar innehållet i detta objekt. |
| [getAlignment()](#getAlignment--) | Hämtar justeringen. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar den senaste ändringstiden. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Hämtar radavståndet. |
| [getParagraphStyle()](#getParagraphStyle--) | Hämtar styckeformatet. |
| [getSpaceAfter()](#getSpaceAfter--) | Hämtar minsta mängd utrymme efter. |
| [getSpaceBefore()](#getSpaceBefore--) | Hämtar minsta mängd utrymme före. |
| [getStyles()](#getStyles--) | Hämtar formaten. |
| [getTags()](#getTags--) | Hämtar listan över alla taggar i ett stycke. |
| [getText()](#getText--) | Hämtar texten. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Returnerar det nollbaserade indexet för den första förekomsten av det angivna Unicode-tecknet i denna sträng. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Returnerar det nollbaserade indexet för den första förekomsten av det angivna Unicode-tecknet i denna sträng. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Returnerar det nollbaserade indexet för den första förekomsten av det angivna tecknet i detta objekt. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i detta objekt. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i detta objekt. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i detta objekt. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det aktuella objektet. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det aktuella objektet. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det aktuella objektet. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Infogar en angiven sträng på en angiven indexposition i detta objekt. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Infogar en angiven sträng med angivet format på en angiven indexposition i detta objekt. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Tar bort alla tecken i det aktuella objektet, med början på en angiven position och fortsätter till den sista positionen. |
| [remove(int startIndex, int count)](#remove-int-int-) | Tar bort ett angivet antal tecken i det aktuella objektet med början på en angiven position. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Ersätter alla förekomster av ett angivet Unicode-tecken i detta objekt med ett annat angivet Unicode-tecken. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersätter alla förekomster av en angiven sträng i det aktuella objektet med en annan angiven sträng. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Ersätter alla förekomster av en angiven sträng i det aktuella objektet med en annan angiven sträng i angivet format. |
| [setAlignment(int value)](#setAlignment-int-) | Ställer in justeringen. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ställer in den senast ändrade tiden. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Ställer in radavståndet. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Ställer in styckeformatet. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Ställer in minsta mängd utrymme efter. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Ställer in minsta mängden utrymme före. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in texten. |
| [trim()](#trim--) | Tar bort alla inledande och avslutande blankstegstecken. |
| [trim(char trimChar)](#trim-char-) | Tar bort alla inledande och avslutande förekomster av ett tecken. |
| [trim(char[] trimChars)](#trim-char...-) | Tar bort alla inledande och avslutande förekomster av en uppsättning tecken som specificeras i en array. |
| [trimEnd()](#trimEnd--) | Tar bort alla avslutande blankstegstecken. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Tar bort alla avslutande förekomster av ett tecken. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Tar bort alla avslutande förekomster av en uppsättning tecken som specificeras i en array. |
| [trimStart()](#trimStart--) | Tar bort alla inledande blankstegstecken. |
| [trimStart(char trimChar)](#trimStart-char-) | Tar bort alla inledande förekomster av ett specificerat tecken. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Tar bort alla inledande förekomster av en uppsättning tecken som specificeras i en array. |
### RichText() {#RichText--}
```
public RichText()
```


Initierar en ny instans av klassen [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är avledd från [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Lägger till en sträng i det sista textintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Det tillagda värdet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Lägger till en sträng i slutet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Det tillagda värdet. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Stilen för den tillagda strängen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Lägger till en sträng i början av det första textintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Det tillagda värdet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Lägger till en sträng i början.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Det tillagda värdet. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Stilen för den tillagda strängen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Rensar innehållet i detta objekt.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Hämtar justeringen.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar den senaste ändringstiden.

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


Hämtar radavståndet.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Hämtar styckeformatet. Dessa inställningar används om det inte finns något matchande TextStyle‑objekt i [getStyles](../../com.aspose.note/richtext\#getStyles)-samlingen eller om detta objekt inte specificerar en behövd inställning.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Hämtar minsta mängd utrymme efter.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Hämtar minsta mängd utrymme före.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Hämtar formaten.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Hämtar listan över alla taggar i ett stycke.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Hämtar texten. Strängen FÅR INTE innehålla några tecken med värdet 10 (radmatning).

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


Returnerar det nollbaserade indexet för den första förekomsten av det angivna Unicode-tecknet i denna sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char | Värdet. |

**Returns:**
int - `int`-typen.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Returnerar det nollbaserade indexet för den första förekomsten av det angivna Unicode‑tecknet i den här strängen. Sökningen startar vid en specificerad teckenposition.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char | Värdet. |
| startIndex | int | Startpositionen för sökningen |

**Returns:**
int - `int`-typen.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Returnerar det nollbaserade indexet för den första förekomsten av det angivna tecknet i detta objekt. Sökningen startar vid en specificerad teckenposition och undersöker ett specificerat antal teckenpositioner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char | Värdet. |
| startIndex | int | Startpositionen för sökningen |
| count | int | Antalet. |

**Returns:**
int - `int`-typen.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Värdet. |

**Returns:**
int - `int`-typen.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i detta objekt. Sökningen startar vid en angiven teckenposition.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Värdet. |
| startIndex | int | Startpositionen för sökningen |

**Returns:**
int - `int`-typen.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i detta objekt. Sökningen startar vid en angiven teckenposition och undersöker ett angivet antal teckenpositioner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Värdet. |
| startIndex | int | Startpositionen för sökningen |
| count | int | Antalet. |

**Returns:**
int - `int`-typen.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det aktuella objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Värdet. |
| startIndex | int | Startpositionen för sökningen |
| count | int | Antalet. |
| comparisonType | short | Typen av sökning som ska användas för den angivna strängen |

**Returns:**
int - `int`-typen.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det aktuella objektet. En parameter anger vilken typ av sökning som ska användas för den angivna strängen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Värdet. |
| comparisonType | short | Typen av sökning som ska användas för den angivna strängen |

**Returns:**
int - `int`-typen.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det aktuella objektet. Parametrar anger startpositionen för sökningen i den aktuella strängen och vilken typ av sökning som ska användas för den angivna strängen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Värdet. |
| startIndex | int | Startpositionen för sökningen |
| comparisonType | short | Typen av sökning som ska användas för den angivna strängen |

**Returns:**
int - `int`-typen.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Infogar en angiven sträng på en angiven indexposition i detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startindexet. |
| värde | java.lang.String | Värdet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Infogar en angiven sträng med angivet format på en angiven indexposition i detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startindexet. |
| värde | java.lang.String | Värdet. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Stilen. |

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


Tar bort alla tecken i det aktuella objektet, med början på en angiven position och fortsätter till den sista positionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startindexet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Tar bort ett angivet antal tecken i det aktuella objektet med början på en angiven position.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startindexet. |
| count | int | Antalet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Ersätter alla förekomster av ett angivet Unicode-tecken i detta objekt med ett annat angivet Unicode-tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldChar | char | Det gamla tecknet. |
| newChar | char | Det nya tecknet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Ersätter alla förekomster av en angiven sträng i det aktuella objektet med en annan angiven sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | java.lang.String | Det gamla värdet. |
| newValue | java.lang.String | Det nya värdet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Ersätter alla förekomster av en angiven sträng i det aktuella objektet med en annan angiven sträng i angivet format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | java.lang.String | Det gamla värdet. |
| newValue | java.lang.String | Det nya värdet. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Stilen för det nya värdet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Ställer in justeringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ställer in den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Ställer in radavståndet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Ställer in stycketstilen. Dessa inställningar används om det inte finns något matchande TextStyle-objekt i [getStyles](../../com.aspose.note/richtext\\#getStyles)-samlingen, eller om detta objekt inte specificerar en nödvändig inställning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Ställer in minsta mängd utrymme efter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Ställer in minsta mängden utrymme före.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Ställer in texten. Strängen FÅR INTE innehålla några tecken med värdet 10 (radmatning).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Tar bort alla inledande och avslutande blankstegstecken.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Tar bort alla inledande och avslutande förekomster av ett tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| trimChar | char | Trimtecknet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Tar bort alla inledande och avslutande förekomster av en uppsättning tecken som specificeras i en array.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| trimChars | char[] | De trimte tecknen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Tar bort alla avslutande blankstegstecken.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Tar bort alla avslutande förekomster av ett tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| trimChar | char | Trimtecknet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Tar bort alla avslutande förekomster av en uppsättning tecken som specificeras i en array.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| trimChars | char[] | De trimte tecknen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Tar bort alla inledande blankstegstecken.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Tar bort alla inledande förekomster av ett specificerat tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| trimChar | char | Trimtecknet. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Tar bort alla inledande förekomster av en uppsättning tecken som specificeras i en array.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| trimChars | char[] | De trimte tecknen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
