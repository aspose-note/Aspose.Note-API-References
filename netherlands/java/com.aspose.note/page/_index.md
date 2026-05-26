---
title: "Page"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een pagina voor."
type: docs
weight: 69
url: /nl/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Stelt een pagina voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Page()](#Page--) | Initialiseert een nieuw exemplaar van de `Page`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [deepClone()](#deepClone--) | Kopieert de pagina. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Kopieert de pagina. |
| [getAuthor()](#getAuthor--) | Haalt de auteur op of stelt deze in. |
| [getBackgroundColor()](#getBackgroundColor--) | Haalt de achtergrondkleur van de pagina op of stelt deze in. |
| [getCreationTime()](#getCreationTime--) | Haalt het aanmaaktijdstip op of stelt het in. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getLevel()](#getLevel--) | Haalt het niveau op of stelt dit in. |
| [getMargin()](#getMargin--) | Haalt de marge op of stelt deze in. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Haalt de revisiesamenvatting voor de pagina en zijn onderliggende knooppunten op of stelt deze in. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Haalt de lay-outgrootte van de pagina op die in de editor wordt weergegeven. |
| [getSizeType()](#getSizeType--) | Haalt het type grootte van een pagina op of stelt dit in. |
| [getTitle()](#getTitle--) | Haalt op of stelt de titel in. |
| [isConflictPage()](#isConflictPage--) | Haalt op of stelt een waarde in die aangeeft of deze pagina een conflictpagina is. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Haalt de auteur op of stelt deze in. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Haalt de achtergrondkleur van de pagina op of stelt deze in. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Haalt op of stelt een waarde in die aangeeft of deze pagina een conflictpagina is. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Haalt het aanmaaktijdstip op of stelt het in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [setLevel(byte value)](#setLevel-byte-) | Haalt het niveau op of stelt dit in. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Haalt de marge op of stelt deze in. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Haalt de revisiesamenvatting voor de pagina en zijn onderliggende knooppunten op of stelt deze in. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Stelt de lay-outgrootte van de pagina in die in de editor wordt weergegeven. |
| [setSizeType(int value)](#setSizeType-int-) | Haalt het type grootte van een pagina op of stelt dit in. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Haalt op of stelt de titel in. |
### Page() {#Page--}
```
public Page()
```


Initialiseert een nieuw exemplaar van de `Page`-klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Kopieert de pagina.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Kopieert de pagina.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cloneHistory | boolean | Specificeert of de geschiedenis van de pagina gekloond moet worden.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Haalt de auteur op of stelt deze in.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Haalt de achtergrondkleur van de pagina op of stelt deze in.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Haalt het aanmaaktijdstip op of stelt het in.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Haalt het niveau op of stelt dit in.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Haalt de marge op of stelt deze in.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Haalt de revisiesamenvatting voor de pagina en zijn onderliggende knooppunten op of stelt deze in.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Haalt de lay-outgrootte van de pagina op die in de editor wordt weergegeven.

--------------------

Deze waarde wordt door de Microsoft OneNote‑applicatie gebruikt om de onderliggende paginalay-out weer te geven wanneer het document wordt geopend. Het heeft verder geen invloed op het afdrukken en opslaan van het document. Wanneer de eigenschap Page.SizeType is ingesteld op PageSizeType.SizeByContent, geeft deze eigenschap de werkelijke grootte van de inhoud terug.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Haalt het type grootte van een pagina op of stelt dit in.

--------------------

Standaard wordt een pagina automatisch aangepast in grootte. De standaardwaarde is [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Haalt op of stelt de titel in.

Waarde: De `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Haalt op of stelt een waarde in die aangeeft of deze pagina een conflictpagina is.

--------------------

De conflictpagina ontstaat wanneer twee gebruikers proberen dezelfde inhoud bij te werken. In dit geval worden de wijzigingen van de eerste gebruiker zoals gewoonlijk geschreven. Maar de wijzigingen van de andere gebruiker kunnen niet worden samengevoegd. Daarom wordt er gewoon een kopie van de pagina gemaakt en gemarkeerd als conflict.

In deze versie worden conflicten opgelost ten gunste van de wijzigingen van de eerste gebruiker. Als een document conflictpagina's bevat, worden deze weergegeven in de geschiedenis, maar overgeslagen bij het opslaan. Het is mogelijk deze vlag te resetten om deze pagina's in de geschiedenis op te slaan als gewone pagina's.

Een gedetailleerd voorbeeld van het manipuleren van een conflictpagina is te vinden in de online documentatie.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Haalt de auteur op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Haalt de achtergrondkleur van de pagina op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Haalt op of stelt een waarde in die aangeeft of deze pagina een conflictpagina is.

--------------------

De conflictpagina ontstaat wanneer twee gebruikers proberen dezelfde inhoud bij te werken. In dit geval worden de wijzigingen van de eerste gebruiker zoals gewoonlijk geschreven. Maar de wijzigingen van de andere gebruiker kunnen niet worden samengevoegd. Daarom wordt er gewoon een kopie van de pagina gemaakt en gemarkeerd als conflict.

In deze versie worden conflicten opgelost ten gunste van de wijzigingen van de eerste gebruiker. Als een document conflictpagina's bevat, worden deze weergegeven in de geschiedenis, maar overgeslagen bij het opslaan. Het is mogelijk deze vlag te resetten om deze pagina's in de geschiedenis op te slaan als gewone pagina's.

Een gedetailleerd voorbeeld van het manipuleren van een conflictpagina is te vinden in de online documentatie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Haalt het aanmaaktijdstip op of stelt het in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Haalt het niveau op of stelt dit in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Haalt de marge op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Haalt de revisiesamenvatting voor de pagina en zijn onderliggende knooppunten op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Stelt de lay-outgrootte van de pagina in die in de editor wordt weergegeven.

--------------------

Deze waarde wordt door de Microsoft OneNote‑applicatie gebruikt om de onderliggende paginalay-out weer te geven wanneer het document wordt geopend. Het heeft verder geen invloed op het afdrukken en opslaan van het document. Wanneer de eigenschap Page.SizeType is ingesteld op PageSizeType.SizeByContent, geeft deze eigenschap de werkelijke grootte van de inhoud terug.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Haalt het type grootte van een pagina op of stelt dit in.

--------------------

Standaard wordt een pagina automatisch aangepast in grootte. De standaardwaarde is [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\\#SizeByContent).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Haalt op of stelt de titel in.

Waarde: De `Title`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

