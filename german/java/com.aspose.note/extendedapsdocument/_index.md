---
title: "ExtendedApsDocument"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt ein vollständiges One-Note-Dokument dar, das aus Seiten besteht, die in Seitensätze übersetzt wurden."
type: docs
weight: 23
url: /de/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

Stellt ein vollständiges OneNote-Dokument dar, das aus Seiten besteht, die in Seitensätze übersetzt wurden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | Initialisiert eine neue Instanz der `ExtendedApsDocument`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | Akzeptiert einen ApsDocumentVisitor für dieses Element. |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | Fügt dem Dokument einen Seitensatz hinzu. |
| [getPageList()](#getPageList--) | Ruft die Liste der Seitensätze ab. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


Initialisiert eine neue Instanz der `ExtendedApsDocument`-Klasse.

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


Akzeptiert einen ApsDocumentVisitor für dieses Element.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Besucher | com.aspose.foundation.rendering.ApsDocumentVisitor | Ein Besucher. |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


Fügt dem Dokument einen Seitensatz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seite | com.aspose.foundation.rendering.ApsPage | Ein Seitensatz. |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


Ruft die Liste der Seitensätze ab.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


Gibt einen Enumerator zurück.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
