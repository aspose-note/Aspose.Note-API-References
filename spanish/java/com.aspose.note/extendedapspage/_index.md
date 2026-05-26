---
title: "ExtendedApsPage"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un contenedor para los ApsGlyphs estándar que extiende parte del comportamiento de dibujo."
type: docs
weight: 27
url: /es/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Representa un contenedor para ApsGlyphs estándar, que extiende parte del comportamiento de dibujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Inicializa una nueva instancia de la clase `ExtendedApsPage`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getContentSize()](#getContentSize--) | Obtiene el tamaño de la página excluyendo los márgenes. |
| [getMargin()](#getMargin--) | Obtiene el margen de esta página. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Obtiene la posición del final de la página, en la página de MS OneNote, cuando una página de MS OneNote se divide en varias páginas aps. |
| [getPageSize()](#getPageSize--) | Obtiene el tamaño final de la página. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Obtiene la posición del inicio de la página en la página de MS OneNote, cuando una página de MS OneNote se divide en varias páginas aps. |
| [iterator()](#iterator--) | Devuelve el enumerador que recorre todos los nodos de esta página. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | El enumerador get. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Inicializa una nueva instancia de la clase `ExtendedApsPage`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | El tamaño de la página. |
| pageStartInNotePage | float | El inicio de la página en la página original de MS OneNote. |
| margin | com.aspose.foundation.layout.Margin | El margen de página extendido. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Obtiene el tamaño de la página excluyendo los márgenes.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Obtiene el margen de esta página.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Obtiene la posición del final de la página, en la página de MS OneNote, cuando una página de MS OneNote se divide en varias páginas aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Obtiene el tamaño final de la página.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Obtiene la posición del inicio de la página en la página de MS OneNote, cuando una página de MS OneNote se divide en varias páginas aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Devuelve el enumerador que recorre todos los nodos de esta página.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - El `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


El enumerador get.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - El `IEnumerator`.
