---
title: "ExtendedApsPage"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een wrapper voor de standaard ApsGlyphs voor die een deel van het teken‑gedrag uitbreidt."
type: docs
weight: 27
url: /nl/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Stelt een wrapper voor de standaard ApsGlyphs voor, die een deel van het teken-gedrag uitbreidt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Initialiseert een nieuw exemplaar van de `ExtendedApsPage`‑klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getContentSize()](#getContentSize--) | Haalt de paginagrootte op exclusief marges. |
| [getMargin()](#getMargin--) | Haalt de marge van deze pagina op. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Haalt de positie van het paginavoor einde op, in de MS OneNote‑pagina, wanneer één MS OneNote‑pagina wordt verdeeld over meerdere aps‑pagina's. |
| [getPageSize()](#getPageSize--) | Haalt de uiteindelijke paginagrootte op. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Haalt de positie van het paginavoor begin op in de MS OneNote‑pagina, wanneer één MS OneNote‑pagina wordt verdeeld over meerdere aps‑pagina's. |
| [iterator()](#iterator--) | Retourneert de enumerator die door alle knooppunten van deze pagina iterereert. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | De get‑enumerator. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Initialiseert een nieuw exemplaar van de `ExtendedApsPage`‑klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | De paginagrootte. |
| pageStartInNotePage | float | Het begin van de pagina in de originele MS OneNote‑pagina. |
| margin | com.aspose.foundation.layout.Margin | The extended page margin. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Haalt de paginagrootte op exclusief marges.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Haalt de marge van deze pagina op.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Haalt de positie van het paginavoor einde op, in de MS OneNote‑pagina, wanneer één MS OneNote‑pagina wordt verdeeld over meerdere aps‑pagina's.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Haalt de uiteindelijke paginagrootte op.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Haalt de positie van het paginavoor begin op in de MS OneNote‑pagina, wanneer één MS OneNote‑pagina wordt verdeeld over meerdere aps‑pagina's.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Retourneert de enumerator die door alle knooppunten van deze pagina iterereert.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - De `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


De get‑enumerator.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - De `IEnumerator`.
