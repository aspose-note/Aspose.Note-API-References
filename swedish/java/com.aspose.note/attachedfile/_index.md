---
title: "AttachedFile"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en bifogad fil."
type: docs
weight: 11
url: /sv/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Representerar en bifogad fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Initierar en ny instans av klassen `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initierar en ny instans av klassen `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Initierar en ny instans av klassen `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initierar en ny instans av klassen `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Initierar en ny instans av klassen `AttachedFile`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getAlignment()](#getAlignment--) | Hämtar justeringen. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Hämtar eller anger en brödtext som alternativ text för ikonen för den bifogade filen. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Hämtar eller anger en titel för alternativ text för ikonen för den bifogade filen. |
| [getBytes()](#getBytes--) | Hämtar binärdata för en inbäddad fil. |
| [getExtension()](#getExtension--) | Hämtar filändelsen för en inbäddad fil. |
| [getFileName()](#getFileName--) | Hämtar namnet på den inbäddade filen. |
| [getFilePath()](#getFilePath--) | Hämtar sökvägen till originalfilen. |
| [getHeight()](#getHeight--) | Hämtar den ursprungliga höjden på ikonen för den inbäddade filen. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Hämtar den horisontella förskjutningen. |
| [getIcon()](#getIcon--) | Hämtar binärdata för ikonen som är associerad med den inbäddade filen. |
| [getIconExtension()](#getIconExtension--) | Hämtar ikons filändelse. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar den senaste ändringstiden. |
| [getMaxHeight()](#getMaxHeight--) | Hämtar den maximala höjden för att visa den inbäddade filikonen. |
| [getMaxWidth()](#getMaxWidth--) | Hämtar den maximala bredden för att visa den inbäddade filikonen. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Hämtar data om felet som inträffade vid åtkomst av filen. |
| [getTags()](#getTags--) | Hämtar listan med taggar för en bifogad fil. |
| [getText()](#getText--) | Hämtar den textuella representationen av den inbäddade filen. |
| [getVerticalOffset()](#getVerticalOffset--) | Hämtar den vertikala förskjutningen. |
| [getWidth()](#getWidth--) | Hämtar den ursprungliga bredden på den inbäddade filikonen. |
| [isPrintout()](#isPrintout--) | Hämtar ett värde som indikerar om filens vy är en utskrift. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Hämtar ett värde som indikerar om ikonens storlek har uppdaterats explicit av användaren. |
| [setAlignment(int value)](#setAlignment-int-) | Ställer in justeringen. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Hämtar eller anger en brödtext som alternativ text för ikonen för den bifogade filen. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Hämtar eller anger en titel för alternativ text för ikonen för den bifogade filen. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Ställer in den horisontella förskjutningen. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ställer in den senast ändrade tiden. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Ställer in den maximala höjden för att visa den inbäddade filikonen. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Ställer in den maximala bredden för att visa den inbäddade filikonen. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Ställer in ett värde som indikerar om filens vy är en utskrift. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Ställer in ett värde som indikerar om ikonens storlek har uppdaterats explicit av användaren. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in den textuella representationen av den inbäddade filen. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Ställer in den vertikala förskjutningen. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Initierar en ny instans av klassen `AttachedFile`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | En sträng som innehåller sökvägen till filen som ska användas för att skapa `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initierar en ny instans av klassen `AttachedFile`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | En sträng som innehåller sökvägen till filen som ska användas för att skapa `AttachedFile`. |
| ikon | java.io.InputStream | En ikon för den bifogade filen. |
| ikonformat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Initierar en ny instans av klassen `AttachedFile`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Ett namn på den bifogade filen. |
| attachedFileStream | java.io.InputStream | En ström som innehåller den bifogade filens byte. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initierar en ny instans av klassen `AttachedFile`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Ett namn på den bifogade filen. |
| attachedFileStream | java.io.InputStream | En ström som innehåller den bifogade filens byte. |
| ikon | java.io.InputStream | En ikon för den bifogade filen. |
| ikonformat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Ett format för den bifogade filikonen. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Initierar en ny instans av klassen `AttachedFile`.

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


Hämtar eller anger en brödtext som alternativ text för ikonen för den bifogade filen.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Hämtar eller anger en titel för alternativ text för ikonen för den bifogade filen.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Hämtar binärdata för en inbäddad fil.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Hämtar filändelsen för en inbäddad fil.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Hämtar namnet på den inbäddade filen.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Hämtar sökvägen till originalfilen.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Hämtar den ursprungliga höjden på ikonen för den inbäddade filen.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Hämtar den horisontella förskjutningen.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Hämtar binärdata för ikonen som är associerad med den inbäddade filen.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Hämtar ikons filändelse.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar den senaste ändringstiden.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Hämtar den maximala höjden för att visa den inbäddade filikonen.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Hämtar den maximala bredden för att visa den inbäddade filikonen.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Hämtar data om felet som inträffade vid åtkomst av filen.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Hämtar listan med taggar för en bifogad fil.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Hämtar textrepresentationen av den inbäddade filen. Strängen FÅR INTE innehålla några tecken med värdet 10 (radmatning) eller 13 (vagnretur).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Hämtar den vertikala förskjutningen.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Hämtar den ursprungliga bredden på den inbäddade filikonen.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Hämtar ett värde som indikerar om filens vy är en utskrift.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Hämtar ett värde som indikerar om ikonens storlek har uppdaterats explicit av användaren.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Ställer in justeringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Justeringens värde. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Hämtar eller anger en brödtext som alternativ text för ikonen för den bifogade filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Hämtar eller anger en titel för alternativ text för ikonen för den bifogade filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Ställer in den horisontella förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | Offsets värde. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ställer in den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | Datumets värde. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Ställer in den maximala höjden för att visa den inbäddade filikonen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | Maximala höjdens värde. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Ställer in den maximala bredden för att visa den inbäddade filikonen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | Maximala breddens värde. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Ställer in ett värde som indikerar om filens vy är en utskrift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | Nytt värde. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Ställer in ett värde som indikerar om ikonens storlek har uppdaterats explicit av användaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | Nytt värde. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ställer in textrepresentationen av den inbäddade filen. Strängen FÅR INTE innehålla några tecken med värdet 10 (radmatning) eller 13 (vagnretur).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Textens värde. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Ställer in den vertikala förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float | Förskjutningens värde. |

