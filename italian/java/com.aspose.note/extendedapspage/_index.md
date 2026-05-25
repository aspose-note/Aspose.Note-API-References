---
title: "ExtendedApsPage"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un wrapper per gli ApsGlyphs standard che estende parte del comportamento di disegno."
type: docs
weight: 27
url: /it/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Rappresenta un wrapper per gli ApsGlyphs standard, che estende parte del comportamento di disegno.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Inizializza una nuova istanza della classe `ExtendedApsPage`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getContentSize()](#getContentSize--) | Ottiene le dimensioni della pagina escludendo i margini. |
| [getMargin()](#getMargin--) | Ottiene il margine di questa pagina. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Ottiene la posizione della fine della pagina, nella pagina MS OneNote, quando una pagina MS OneNote è divisa in più pagine aps. |
| [getPageSize()](#getPageSize--) | Ottiene le dimensioni finali della pagina. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Ottiene la posizione dell'inizio della pagina nella pagina MS OneNote, quando una pagina MS OneNote è divisa in più pagine aps. |
| [iterator()](#iterator--) | Restituisce l'enumeratore che itera attraverso tutti i nodi di questa pagina. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | L'enumeratore get. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Inizializza una nuova istanza della classe `ExtendedApsPage`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Le dimensioni della pagina. |
| pageStartInNotePage | float | L'inizio della pagina nella pagina MS OneNote originale. |
| margin | com.aspose.foundation.layout.Margin | Il margine di pagina esteso. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Ottiene le dimensioni della pagina escludendo i margini.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Ottiene il margine di questa pagina.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Ottiene la posizione della fine della pagina, nella pagina MS OneNote, quando una pagina MS OneNote è divisa in più pagine aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Ottiene le dimensioni finali della pagina.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Ottiene la posizione dell'inizio della pagina nella pagina MS OneNote, quando una pagina MS OneNote è divisa in più pagine aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Restituisce l'enumeratore che itera attraverso tutti i nodi di questa pagina.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Il `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


L'enumeratore get.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Il `IEnumerator`.
