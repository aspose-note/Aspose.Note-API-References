---
title: "Bild"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en bild."
type: docs
weight: 33
url: /sv/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Representerar en bild.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Initierar en ny instans av klassen `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Initierar en ny instans av klassen `Image`. |
| [Image()](#Image--) | Initierar en ny instans av klassen `Image`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getAlignment()](#getAlignment--) | Hämtar justeringen. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Hämtar en brödtext för den alternativa texten för bilden. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Hämtar en titel för den alternativa texten för bilden. |
| [getBytes()](#getBytes--) | Hämtar bildens datalager. |
| [getFileName()](#getFileName--) | Hämtar filnamnet. |
| [getFilePath()](#getFilePath--) | Hämtar sökvägen till bildfilen. |
| [getFormat()](#getFormat--) | Hämtar bildens format. |
| [getHeight()](#getHeight--) | Hämtar höjden. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Hämtar den horisontella förskjutningen. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Hämtar hyperlänken som är associerad med bilden. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar senast ändrad tid. |
| [getOriginalHeight()](#getOriginalHeight--) | Hämtar den ursprungliga höjden. |
| [getOriginalWidth()](#getOriginalWidth--) | Hämtar den ursprungliga bredden. |
| [getTags()](#getTags--) | Hämtar listan med alla taggar för en bild. |
| [getVerticalOffset()](#getVerticalOffset--) | Hämtar den vertikala förskjutningen. |
| [getWidth()](#getWidth--) | Hämtar bredden. |
| [isBackground()](#isBackground--) | Hämtar om bilden är en bakgrundsbild. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Ersätter den aktuella bilddatan med data från det angivna Image-objektet. |
| [setAlignment(int value)](#setAlignment-int-) | Ställer in justeringen. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Ställer in en brödtext för den alternativa texten för bilden. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Ställer in en titel för den alternativa texten för bilden. |
| [setBackground(boolean value)](#setBackground-boolean-) | Hämtar om bilden är en bakgrundsbild. |
| [setHeight(float value)](#setHeight-float-) | Ställer in höjden. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Ställer in den horisontella förskjutningen. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Ställer in hyperlänken som är associerad med bilden. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ställer in senast ändrad tid. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Ställer in den vertikala förskjutningen. |
| [setWidth(float value)](#setWidth-float-) | Ställer in bredden. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Initierar en ny instans av klassen `Image`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | En sträng som innehåller sökvägen till filen från vilken `Image` ska skapas. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Initierar en ny instans av klassen `Image`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Ett namn på bilden. |
| imageStream | java.io.InputStream | En ström som innehåller bilden. |

### Image() {#Image--}
```
public Image()
```


Initierar en ny instans av klassen `Image`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Hämtar justeringen.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Hämtar en brödtext för den alternativa texten för bilden.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Hämtar en titel för den alternativa texten för bilden.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Hämtar bildens datalager.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Hämtar filnamnet.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Hämtar sökvägen till bildfilen.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Hämtar bildens format.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Hämtar höjden. Detta är den faktiska höjden på bilden i MS OneNote-dokumentet.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Hämtar den horisontella förskjutningen.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Hämtar hyperlänken som är associerad med bilden.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar senast ändrad tid.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Hämtar den ursprungliga höjden. Detta är den ursprungliga bredden på bilden, innan storleksändring.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Hämtar den ursprungliga bredden. Detta är den ursprungliga bredden på bilden, innan storleksändring.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Hämtar listan med alla taggar för en bild.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Hämtar den vertikala förskjutningen.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Hämtar bredden. Detta är den faktiska bredden på bilden i MS OneNote-dokumentet.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Hämtar om bilden är en bakgrundsbild.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Ersätter den aktuella bilddatan med data från det angivna Image-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Ställer in justeringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Ställer in en brödtext för den alternativa texten för bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Ställer in en titel för den alternativa texten för bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Hämtar om bilden är en bakgrundsbild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Ställer in höjden. Detta är den faktiska höjden på bilden i MS OneNote-dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Ställer in den horisontella förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Ställer in hyperlänken som är associerad med bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ställer in senast ändrad tid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Ställer in den vertikala förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Ställer in bredden. Detta är den faktiska bredden på bilden i MS OneNote-dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

