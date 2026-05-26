---
title: "Afbeelding"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een afbeelding voor."
type: docs
weight: 33
url: /nl/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Stelt een afbeelding voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Initialiseert een nieuw exemplaar van de `Image`-klasse. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de `Image`-klasse. |
| [Image()](#Image--) | Initialiseert een nieuw exemplaar van de `Image`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getAlignment()](#getAlignment--) | Haalt de uitlijning op. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Haalt een body en alternatieve tekst voor de afbeelding op. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Haalt een titel van de alternatieve tekst voor de afbeelding op. |
| [getBytes()](#getBytes--) | Haalt de afbeeldingsdatastore op. |
| [getFileName()](#getFileName--) | Haalt de bestandsnaam op. |
| [getFilePath()](#getFilePath--) | Haalt het pad naar het afbeeldingsbestand op. |
| [getFormat()](#getFormat--) | Haalt het formaat van de afbeelding op. |
| [getHeight()](#getHeight--) | Haalt de hoogte op. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Haalt de horizontale offset op. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Haalt de hyperlink op die aan de afbeelding is gekoppeld. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt de laatst gewijzigde tijd op. |
| [getOriginalHeight()](#getOriginalHeight--) | Haalt de oorspronkelijke hoogte op. |
| [getOriginalWidth()](#getOriginalWidth--) | Haalt de oorspronkelijke breedte op. |
| [getTags()](#getTags--) | Haalt de lijst met alle tags van een afbeelding op. |
| [getVerticalOffset()](#getVerticalOffset--) | Haalt de verticale offset op. |
| [getWidth()](#getWidth--) | Haalt de breedte op. |
| [isBackground()](#isBackground--) | Haalt op of de afbeelding een achtergrondafbeelding is. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Vervangt de huidige afbeeldingsgegevens door de gegevens van het opgegeven Image-object. |
| [setAlignment(int value)](#setAlignment-int-) | Stelt de uitlijning in. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Stelt een body en alternatieve tekst voor de afbeelding in. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Stelt een titel van de alternatieve tekst voor de afbeelding in. |
| [setBackground(boolean value)](#setBackground-boolean-) | Haalt op of de afbeelding een achtergrondafbeelding is. |
| [setHeight(float value)](#setHeight-float-) | Stelt de hoogte in. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Stelt de horizontale offset in. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Stelt de hyperlink in die aan de afbeelding is gekoppeld. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Stelt de laatste wijzigingstijd in. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Stelt de verticale offset in. |
| [setWidth(float value)](#setWidth-float-) | Stelt de breedte in. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Initialiseert een nieuw exemplaar van de `Image`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Een string die het pad naar het bestand bevat waaruit de `Image` wordt gemaakt. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Initialiseert een nieuw exemplaar van de `Image`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Een naam van de afbeelding. |
| imageStream | java.io.InputStream | Een stream die de afbeelding bevat. |

### Image() {#Image--}
```
public Image()
```


Initialiseert een nieuw exemplaar van de `Image`-klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Haalt de uitlijning op.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Haalt een body en alternatieve tekst voor de afbeelding op.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Haalt een titel van de alternatieve tekst voor de afbeelding op.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Haalt de afbeeldingsdatastore op.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Haalt de bestandsnaam op.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Haalt het pad naar het afbeeldingsbestand op.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Haalt het formaat van de afbeelding op.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Haalt de hoogte op. Dit is de werkelijke hoogte van de afbeelding in het MS OneNote-document.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Haalt de horizontale offset op.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Haalt de hyperlink op die aan de afbeelding is gekoppeld.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt de laatst gewijzigde tijd op.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Haalt de oorspronkelijke hoogte op. Dit is de oorspronkelijke breedte van de afbeelding, vóór het schalen.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Haalt de oorspronkelijke breedte op. Dit is de oorspronkelijke breedte van de afbeelding, vóór het schalen.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Haalt de lijst met alle tags van een afbeelding op.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Haalt de verticale offset op.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Haalt de breedte op. Dit is de werkelijke breedte van de afbeelding in het MS OneNote-document.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Haalt op of de afbeelding een achtergrondafbeelding is.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Vervangt de huidige afbeeldingsgegevens door de gegevens van het opgegeven Image-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Stelt de uitlijning in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Stelt een body en alternatieve tekst voor de afbeelding in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Stelt een titel van de alternatieve tekst voor de afbeelding in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Haalt op of de afbeelding een achtergrondafbeelding is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Stelt de hoogte in. Dit is de werkelijke hoogte van de afbeelding in het MS OneNote-document.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Stelt de horizontale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Stelt de hyperlink in die aan de afbeelding is gekoppeld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Stelt de laatste wijzigingstijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Stelt de verticale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Stelt de breedte in. Dit is de werkelijke breedte van de afbeelding in het MS OneNote-document.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

