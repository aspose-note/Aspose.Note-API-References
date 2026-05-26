---
title: "ExtendedApsDocument"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un documento completo de una sola nota compuesto por páginas traducidas en conjuntos de páginas."
type: docs
weight: 23
url: /es/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

Representa un documento OneNote completo, compuesto por páginas traducidas en conjuntos de páginas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | Inicializa una nueva instancia de la clase `ExtendedApsDocument`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | Acepta ApsDocumentVisitor a este elemento. |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | Agrega un conjunto de páginas al documento. |
| [getPageList()](#getPageList--) | Obtiene la lista de conjuntos de páginas. |
| [iterator()](#iterator--) | Devuelve un enumerador. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


Inicializa una nueva instancia de la clase `ExtendedApsDocument`.

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


Acepta ApsDocumentVisitor a este elemento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitante | com.aspose.foundation.rendering.ApsDocumentVisitor | Un visitante. |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


Agrega un conjunto de páginas al documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| página | com.aspose.foundation.rendering.ApsPage | Un conjunto de páginas. |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


Obtiene la lista de conjuntos de páginas.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


Devuelve un enumerador.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
