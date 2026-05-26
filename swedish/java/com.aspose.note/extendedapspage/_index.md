---
title: "ExtendedApsPage"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en wrapper för de standard ApsGlyphs som utökar viss ritningsbeteende."
type: docs
weight: 27
url: /sv/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Representerar en wrapper för standard-ApsGlyphs, som utökar viss ritbeteende.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Initierar en ny instans av klassen `ExtendedApsPage`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getContentSize()](#getContentSize--) | Hämtar sidans storlek exklusive marginaler. |
| [getMargin()](#getMargin--) | Hämtar marginalen för den här sidan. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Hämtar positionen för sidans slut, i MS OneNote-sidan, när en MS OneNote-sida delas upp i flera aps-sidor. |
| [getPageSize()](#getPageSize--) | Hämtar den slutgiltiga sidstorleken. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Hämtar positionen för sidans början i MS OneNote-sidan, när en MS OneNote-sida delas upp i flera aps-sidor. |
| [iterator()](#iterator--) | Returnerar enumeratorn som itererar genom alla noder från den här sidan. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | Get-enumeratorn. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Initierar en ny instans av klassen `ExtendedApsPage`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Sidans storlek. |
| pageStartInNotePage | float | Sidans början i den ursprungliga MS OneNote-sidan. |
| margin | com.aspose.foundation.layout.Margin | Den utökade sidmarginalen. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Hämtar sidans storlek exklusive marginaler.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Hämtar marginalen för den här sidan.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Hämtar positionen för sidans slut, i MS OneNote-sidan, när en MS OneNote-sida delas upp i flera aps-sidor.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Hämtar den slutgiltiga sidstorleken.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Hämtar positionen för sidans början i MS OneNote-sidan, när en MS OneNote-sida delas upp i flera aps-sidor.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Returnerar enumeratorn som itererar genom alla noder från den här sidan.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Den `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


Get-enumeratorn.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Den `IEnumerator`.
