---
title: "Page"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en sida."
type: docs
weight: 69
url: /sv/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Representerar en sida.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Page()](#Page--) | Initierar en ny instans av klassen `Page`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [deepClone()](#deepClone--) | Klonar sidan. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Klonar sidan. |
| [getAuthor()](#getAuthor--) | Hämtar eller anger författaren. |
| [getBackgroundColor()](#getBackgroundColor--) | Hämtar eller anger sidans bakgrundsfärg. |
| [getCreationTime()](#getCreationTime--) | Hämtar eller anger skapningstiden. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar eller anger den senast ändrade tiden. |
| [getLevel()](#getLevel--) | Hämtar eller anger nivån. |
| [getMargin()](#getMargin--) | Hämtar eller anger marginalen. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Hämtar eller anger revisionssammanfattningen för sidan och dess barnnoder. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Hämtar sidans layoutstorlek som visas i redigeraren. |
| [getSizeType()](#getSizeType--) | Hämtar eller anger storlekstypen för en sida. |
| [getTitle()](#getTitle--) | Hämtar eller anger titeln. |
| [isConflictPage()](#isConflictPage--) | Hämtar eller anger ett värde som indikerar om den här sidan är en konfliktssida. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Hämtar eller anger författaren. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Hämtar eller anger sidans bakgrundsfärg. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Hämtar eller anger ett värde som indikerar om den här sidan är en konfliktssida. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Hämtar eller anger skapningstiden. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Hämtar eller anger den senast ändrade tiden. |
| [setLevel(byte value)](#setLevel-byte-) | Hämtar eller anger nivån. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Hämtar eller anger marginalen. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Hämtar eller anger revisionssammanfattningen för sidan och dess barnnoder. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Anger sidans layoutstorlek som visas i redigeraren. |
| [setSizeType(int value)](#setSizeType-int-) | Hämtar eller anger storlekstypen för en sida. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Hämtar eller anger titeln. |
### Page() {#Page--}
```
public Page()
```


Initierar en ny instans av klassen `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Klonar sidan.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Klonar sidan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cloneHistory | boolean | Anger om sidans historik ska klonas.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Hämtar eller anger författaren.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Hämtar eller anger sidans bakgrundsfärg.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Hämtar eller anger skapningstiden.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar eller anger den senast ändrade tiden.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Hämtar eller anger nivån.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Hämtar eller anger marginalen.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Hämtar eller anger revisionssammanfattningen för sidan och dess barnnoder.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Hämtar sidans layoutstorlek som visas i redigeraren.

--------------------

Detta värde används av Microsoft OneNote‑applikationen för att visa underliggande sidlayout när dokumentet öppnas. Det påverkar inte utskrift och sparande av dokumentet ändå. När egenskapen Page.SizeType är satt till PageSizeType.SizeByContent returnerar denna egenskap den faktiska storleken på innehållet.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Hämtar eller anger storlekstypen för en sida.

--------------------

Som standard ändras en sida automatiskt i storlek. Standardvärdet är [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Hämtar eller anger titeln.

Värde: `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Hämtar eller anger ett värde som indikerar om den här sidan är en konfliktssida.

--------------------

Konfliktssidan uppstår när två användare försöker uppdatera samma innehåll. I detta fall skrivs den första användarens ändringar som vanligt. Men ändringarna från den andra användaren kan inte slås ihop. Så en kopia av sidan skapas och markeras som konflikt.

I den här versionen löses konflikterna till förmån för den första användarens ändringar. Så om dokumentet har konfliktssidor kommer de att visas i historiken men de kommer att hoppas över vid sparande. Det är möjligt att återställa denna flagga för att spara dessa sidor i historiken som vanliga.

Detaljerat exempel på hantering av konfliktssidor finns i den online‑dokumentationen.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Hämtar eller anger författaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Hämtar eller anger sidans bakgrundsfärg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Hämtar eller anger ett värde som indikerar om den här sidan är en konfliktssida.

--------------------

Konfliktssidan uppstår när två användare försöker uppdatera samma innehåll. I detta fall skrivs den första användarens ändringar som vanligt. Men ändringarna från den andra användaren kan inte slås ihop. Så en kopia av sidan skapas och markeras som konflikt.

I den här versionen löses konflikterna till förmån för den första användarens ändringar. Så om dokumentet har konfliktssidor kommer de att visas i historiken men de kommer att hoppas över vid sparande. Det är möjligt att återställa denna flagga för att spara dessa sidor i historiken som vanliga.

Detaljerat exempel på hantering av konfliktssidor finns i den online‑dokumentationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Hämtar eller anger skapningstiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Hämtar eller anger den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Hämtar eller anger nivån.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Hämtar eller anger marginalen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Hämtar eller anger revisionssammanfattningen för sidan och dess barnnoder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Anger sidans layoutstorlek som visas i redigeraren.

--------------------

Detta värde används av Microsoft OneNote‑applikationen för att visa underliggande sidlayout när dokumentet öppnas. Det påverkar inte utskrift och sparande av dokumentet ändå. När egenskapen Page.SizeType är satt till PageSizeType.SizeByContent returnerar denna egenskap den faktiska storleken på innehållet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Hämtar eller anger storlekstypen för en sida.

--------------------

Som standard ändras en sida automatiskt i storlek. Standardvärdet är [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Hämtar eller anger titeln.

Värde: `Title`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

