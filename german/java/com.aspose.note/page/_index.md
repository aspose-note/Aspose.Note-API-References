---
title: "Page"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt eine Seite dar."
type: docs
weight: 69
url: /de/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Stellt eine Seite dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Page()](#Page--) | Initialisiert eine neue Instanz der `Page`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [deepClone()](#deepClone--) | Kopiert die Seite. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Kopiert die Seite. |
| [getAuthor()](#getAuthor--) | Liest oder setzt den Autor. |
| [getBackgroundColor()](#getBackgroundColor--) | Liest oder setzt die Hintergrundfarbe der Seite. |
| [getCreationTime()](#getCreationTime--) | Liest oder setzt die Erstellungszeit. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest oder setzt die zuletzt geänderte Zeit. |
| [getLevel()](#getLevel--) | Liest oder setzt das Level. |
| [getMargin()](#getMargin--) | Liest oder setzt den Rand. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Liest oder setzt die Revisionszusammenfassung für die Seite und ihre Kindknoten. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Liest die Layoutgröße der Seite, die im Editor angezeigt wird. |
| [getSizeType()](#getSizeType--) | Liest oder setzt den Größentyp einer Seite. |
| [getTitle()](#getTitle--) | Liest oder setzt den Titel. |
| [isConflictPage()](#isConflictPage--) | Liest oder setzt einen Wert, der angibt, ob diese Seite eine Konfliktseite ist. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Liest oder setzt den Autor. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Liest oder setzt die Hintergrundfarbe der Seite. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Liest oder setzt einen Wert, der angibt, ob diese Seite eine Konfliktseite ist. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Liest oder setzt die Erstellungszeit. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Liest oder setzt die zuletzt geänderte Zeit. |
| [setLevel(byte value)](#setLevel-byte-) | Liest oder setzt das Level. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Liest oder setzt den Rand. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Liest oder setzt die Revisionszusammenfassung für die Seite und ihre Kindknoten. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Setzt die im Editor angezeigte Layoutgröße der Seite. |
| [setSizeType(int value)](#setSizeType-int-) | Liest oder setzt den Größentyp einer Seite. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Liest oder setzt den Titel. |
### Page() {#Page--}
```
public Page()
```


Initialisiert eine neue Instanz der `Page`-Klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Kopiert die Seite.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Kopiert die Seite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cloneHistory | boolean | Gibt an, ob die Historie der Seite geklont werden soll.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Liest oder setzt den Autor.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Liest oder setzt die Hintergrundfarbe der Seite.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Liest oder setzt die Erstellungszeit.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest oder setzt die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Liest oder setzt das Level.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Liest oder setzt den Rand.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Liest oder setzt die Revisionszusammenfassung für die Seite und ihre Kindknoten.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Liest die Layoutgröße der Seite, die im Editor angezeigt wird.

--------------------

Dieser Wert wird von der Microsoft OneNote-Anwendung verwendet, um das zugrunde liegende Seitenlayout anzuzeigen, wenn das Dokument geöffnet wird. Er beeinflusst das Drucken und Speichern des Dokuments jedoch nicht. Wenn die Eigenschaft Page.SizeType auf PageSizeType.SizeByContent gesetzt ist, gibt diese Eigenschaft die tatsächliche Größe des Inhalts zurück.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Liest oder setzt den Größentyp einer Seite.

--------------------

Standardmäßig wird die Größe einer Seite automatisch angepasst. Der Standardwert ist [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Liest oder setzt den Titel.

Wert: Der `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Liest oder setzt einen Wert, der angibt, ob diese Seite eine Konfliktseite ist.

--------------------

Die Konfliktseite entsteht, wenn zwei Benutzer versuchen, denselben Inhalt zu aktualisieren. In diesem Fall werden die Änderungen des ersten Benutzers wie gewohnt geschrieben. Die Änderungen eines anderen Benutzers können jedoch nicht zusammengeführt werden. Daher wird einfach eine Kopie der Seite erstellt und als Konflikt markiert.

In dieser Version werden Konflikte zugunsten der Änderungen des ersten Benutzers gelöst. Wenn ein Dokument Konfliktseiten enthält, werden diese in der Historie angezeigt, beim Speichern jedoch übersprungen. Es ist möglich, dieses Flag zurückzusetzen, um diese Seiten in der Historie wie gewöhnliche Seiten zu speichern.

Ein ausführliches Beispiel zur Manipulation von Konfliktseiten ist in der Online-Dokumentation zu finden.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Liest oder setzt den Autor.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Liest oder setzt die Hintergrundfarbe der Seite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob diese Seite eine Konfliktseite ist.

--------------------

Die Konfliktseite entsteht, wenn zwei Benutzer versuchen, denselben Inhalt zu aktualisieren. In diesem Fall werden die Änderungen des ersten Benutzers wie gewohnt geschrieben. Die Änderungen eines anderen Benutzers können jedoch nicht zusammengeführt werden. Daher wird einfach eine Kopie der Seite erstellt und als Konflikt markiert.

In dieser Version werden Konflikte zugunsten der Änderungen des ersten Benutzers gelöst. Wenn ein Dokument Konfliktseiten enthält, werden diese in der Historie angezeigt, beim Speichern jedoch übersprungen. Es ist möglich, dieses Flag zurückzusetzen, um diese Seiten in der Historie wie gewöhnliche Seiten zu speichern.

Ein ausführliches Beispiel zur Manipulation von Konfliktseiten ist in der Online-Dokumentation zu finden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Liest oder setzt die Erstellungszeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Liest oder setzt die zuletzt geänderte Zeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Liest oder setzt das Level.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Liest oder setzt den Rand.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Liest oder setzt die Revisionszusammenfassung für die Seite und ihre Kindknoten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Setzt die im Editor angezeigte Layoutgröße der Seite.

--------------------

Dieser Wert wird von der Microsoft OneNote-Anwendung verwendet, um das zugrunde liegende Seitenlayout anzuzeigen, wenn das Dokument geöffnet wird. Er beeinflusst das Drucken und Speichern des Dokuments jedoch nicht. Wenn die Eigenschaft Page.SizeType auf PageSizeType.SizeByContent gesetzt ist, gibt diese Eigenschaft die tatsächliche Größe des Inhalts zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Liest oder setzt den Größentyp einer Seite.

--------------------

Standardmäßig wird die Größe einer Seite automatisch angepasst. Der Standardwert ist [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Liest oder setzt den Titel.

Wert: Der `Title`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

