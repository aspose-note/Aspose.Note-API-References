---
title: "ExtendedApsDocument"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar ett fullständigt one-note-dokument bestående av Pages som översatts till siduppsättningar."
type: docs
weight: 23
url: /sv/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

Representerar ett fullständigt OneNote-dokument, bestående av sidor som översatts till siduppsättningar.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | Initierar en ny instans av klassen `ExtendedApsDocument`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | Accepterar ApsDocumentVisitor för detta element. |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | Lägger till en siduppsättning till dokumentet. |
| [getPageList()](#getPageList--) | Hämtar listan med siduppsättningar. |
| [iterator()](#iterator--) | Returnerar en enumerator. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


Initierar en ny instans av klassen `ExtendedApsDocument`.

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


Accepterar ApsDocumentVisitor för detta element.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| besökare | com.aspose.foundation.rendering.ApsDocumentVisitor | En besökare. |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


Lägger till en siduppsättning till dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sida | com.aspose.foundation.rendering.ApsPage | En siduppsättning. |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


Hämtar listan med siduppsättningar.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


Returnerar en enumerator.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
