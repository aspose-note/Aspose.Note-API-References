---
title: "AttachedFile"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een bijgevoegd bestand voor."
type: docs
weight: 11
url: /nl/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Stelt een bijgevoegd bestand voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse. |
| [AttachedFile()](#AttachedFile--) | Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getAlignment()](#getAlignment--) | Haalt de uitlijning op. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Haalt op of stelt een alternatieve tekst voor het pictogram van het bijgevoegde bestand in. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Haalt op of stelt een titel van alternatieve tekst voor het pictogram van het bijgevoegde bestand in. |
| [getBytes()](#getBytes--) | Haalt de binaire gegevens op voor een ingebed bestand. |
| [getExtension()](#getExtension--) | Haalt de extensie op van een ingebed bestand. |
| [getFileName()](#getFileName--) | Haalt de naam op van een ingebed bestand. |
| [getFilePath()](#getFilePath--) | Haalt het pad op naar het originele bestand. |
| [getHeight()](#getHeight--) | Haalt de oorspronkelijke hoogte op van het pictogram van het ingebedde bestand. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Haalt de horizontale offset op. |
| [getIcon()](#getIcon--) | Haalt de binaire gegevens op voor het pictogram dat is gekoppeld aan het ingebedde bestand. |
| [getIconExtension()](#getIconExtension--) | Haalt de extensie op van het pictogram. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt de laatst gewijzigde tijd op. |
| [getMaxHeight()](#getMaxHeight--) | Haalt de maximale hoogte op om het ingesloten bestandspictogram weer te geven. |
| [getMaxWidth()](#getMaxWidth--) | Haalt de maximale breedte op om het ingesloten bestandspictogram weer te geven. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Haalt de gegevens over de fout op die optrad tijdens het openen van het bestand. |
| [getTags()](#getTags--) | Haalt de lijst met tags van een bijgevoegd bestand op. |
| [getText()](#getText--) | Haalt de tekstrepresentatie van het ingesloten bestand op. |
| [getVerticalOffset()](#getVerticalOffset--) | Haalt de verticale offset op. |
| [getWidth()](#getWidth--) | Haalt de oorspronkelijke breedte van het ingesloten bestandspictogram op. |
| [isPrintout()](#isPrintout--) | Haalt een waarde op die aangeeft of de weergave van het bestand een afdruk is. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Haalt een waarde op die aangeeft of de grootte van het pictogram expliciet door de gebruiker is bijgewerkt. |
| [setAlignment(int value)](#setAlignment-int-) | Stelt de uitlijning in. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Haalt op of stelt een alternatieve tekst voor het pictogram van het bijgevoegde bestand in. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Haalt op of stelt een titel van alternatieve tekst voor het pictogram van het bijgevoegde bestand in. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Stelt de horizontale offset in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Stelt de laatst gewijzigde tijd in. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Stelt de maximale hoogte in om het ingesloten bestandspictogram weer te geven. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Stelt de maximale breedte in om het ingesloten bestandspictogram weer te geven. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Stelt een waarde in die aangeeft of de weergave van het bestand een afdruk is. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Stelt een waarde in die aangeeft of de grootte van het pictogram expliciet door de gebruiker is bijgewerkt. |
| [setText(String value)](#setText-java.lang.String-) | Stelt de tekstrepresentatie van het ingesloten bestand in. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Stelt de verticale offset in. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Een tekenreeks die het pad bevat naar het bestand waaruit de `AttachedFile` moet worden gemaakt. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Een tekenreeks die het pad bevat naar het bestand waaruit de `AttachedFile` moet worden gemaakt. |
| icon | java.io.InputStream | Een pictogram voor het bijgevoegde bestand. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Een naam van het bijgevoegde bestand. |
| attachedFileStream | java.io.InputStream | Een stream die de bytes van het bijgevoegde bestand bevat. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Een naam van het bijgevoegde bestand. |
| attachedFileStream | java.io.InputStream | Een stream die de bytes van het bijgevoegde bestand bevat. |
| icon | java.io.InputStream | Een pictogram voor het bijgevoegde bestand. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Een formaat van het pictogram van het bijgevoegde bestand. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Initialiseert een nieuw exemplaar van de `AttachedFile`-klasse.

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


Haalt op of stelt een alternatieve tekst voor het pictogram van het bijgevoegde bestand in.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Haalt op of stelt een titel van alternatieve tekst voor het pictogram van het bijgevoegde bestand in.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Haalt de binaire gegevens op voor een ingebed bestand.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Haalt de extensie op van een ingebed bestand.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Haalt de naam op van een ingebed bestand.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Haalt het pad op naar het originele bestand.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Haalt de oorspronkelijke hoogte op van het pictogram van het ingebedde bestand.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Haalt de horizontale offset op.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Haalt de binaire gegevens op voor het pictogram dat is gekoppeld aan het ingebedde bestand.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Haalt de extensie op van het pictogram.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt de laatst gewijzigde tijd op.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Haalt de maximale hoogte op om het ingesloten bestandspictogram weer te geven.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Haalt de maximale breedte op om het ingesloten bestandspictogram weer te geven.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Haalt de gegevens over de fout op die optrad tijdens het openen van het bestand.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Haalt de lijst met tags van een bijgevoegd bestand op.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Haalt de tekstrepresentatie van het ingebedde bestand op. De string MAG GEEN tekens bevatten met de waarde 10 (regelvoeding) of 13 (carriage return).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Haalt de verticale offset op.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Haalt de oorspronkelijke breedte van het ingesloten bestandspictogram op.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Haalt een waarde op die aangeeft of de weergave van het bestand een afdruk is.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Haalt een waarde op die aangeeft of de grootte van het pictogram expliciet door de gebruiker is bijgewerkt.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Stelt de uitlijning in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | Waarde van Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Haalt op of stelt een alternatieve tekst voor het pictogram van het bijgevoegde bestand in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Haalt op of stelt een titel van alternatieve tekst voor het pictogram van het bijgevoegde bestand in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Stelt de horizontale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | Waarde van Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | Waarde van Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Stelt de maximale hoogte in om het ingesloten bestandspictogram weer te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | Waarde van Maximum height. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Stelt de maximale breedte in om het ingesloten bestandspictogram weer te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | Waarde van Maximum width. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Stelt een waarde in die aangeeft of de weergave van het bestand een afdruk is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | Nieuwe waarde. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Stelt een waarde in die aangeeft of de grootte van het pictogram expliciet door de gebruiker is bijgewerkt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | Nieuwe waarde. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Stelt de tekstrepresentatie van het ingebedde bestand in. De string MAG GEEN tekens bevatten met de waarde 10 (regelvoeding) of 13 (carriage return).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | Waarde van Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Stelt de verticale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float | Waarde van Offset. |

