---
title: "ExtendedApsDocument"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een volledig one-note document voor dat bestaat uit pagina's vertaald naar paginagroepen."
type: docs
weight: 23
url: /nl/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

Stelt een volledig OneNote-document voor, bestaande uit Pagina's die zijn vertaald naar pagina-sets.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | Initialiseert een nieuw exemplaar van de `ExtendedApsDocument` klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | Accepteert ApsDocumentVisitor voor dit element. |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | Voegt een paginagroep toe aan het document. |
| [getPageList()](#getPageList--) | Haalt de lijst met paginagroepen op. |
| [iterator()](#iterator--) | Retourneert een enumerator. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


Initialiseert een nieuw exemplaar van de `ExtendedApsDocument` klasse.

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


Accepteert ApsDocumentVisitor voor dit element.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bezoeker | com.aspose.foundation.rendering.ApsDocumentVisitor | Een bezoeker. |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


Voegt een paginagroep toe aan het document.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pagina | com.aspose.foundation.rendering.ApsPage | Een paginagroep. |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


Haalt de lijst met paginagroepen op.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


Retourneert een enumerator.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
