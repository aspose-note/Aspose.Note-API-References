---
title: "ExtendedApsPage"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Wrapper für die Standard‑ApsGlyphs dar, der einige Zeichenverhalten erweitert."
type: docs
weight: 27
url: /de/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Stellt einen Wrapper für die standardmäßigen ApsGlyphs dar, der das Zeichenverhalten erweitert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Initialisiert eine neue Instanz der Klasse `ExtendedApsPage`. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getContentSize()](#getContentSize--) | Liest die Seitengröße ohne Rand. |
| [getMargin()](#getMargin--) | Liest den Rand dieser Seite. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Liest die Position des Seitenendes in der MS‑OneNote‑Seite, wenn eine MS‑OneNote‑Seite in mehrere aps‑Seiten aufgeteilt wird. |
| [getPageSize()](#getPageSize--) | Liest die endgültige Seitengröße. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Liest die Position des Seitenanfangs in der MS‑OneNote‑Seite, wenn eine MS‑OneNote‑Seite in mehrere aps‑Seiten aufgeteilt wird. |
| [iterator()](#iterator--) | Gibt den Enumerator zurück, der alle Knoten dieser Seite durchläuft. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | Der Get‑Enumerator. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Initialisiert eine neue Instanz der Klasse `ExtendedApsPage`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Die Seitengröße. |
| pageStartInNotePage | float | Der Seitenanfang in der ursprünglichen MS‑OneNote‑Seite. |
| margin | com.aspose.foundation.layout.Margin | Der erweiterte Seitenrand. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Liest die Seitengröße ohne Rand.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Liest den Rand dieser Seite.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Liest die Position des Seitenendes in der MS‑OneNote‑Seite, wenn eine MS‑OneNote‑Seite in mehrere aps‑Seiten aufgeteilt wird.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Liest die endgültige Seitengröße.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Liest die Position des Seitenanfangs in der MS‑OneNote‑Seite, wenn eine MS‑OneNote‑Seite in mehrere aps‑Seiten aufgeteilt wird.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Gibt den Enumerator zurück, der alle Knoten dieser Seite durchläuft.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Der `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


Der Get‑Enumerator.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Der `IEnumerator`.
