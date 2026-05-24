---
title: "ExtendedApsPage"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un wrapper pour les ApsGlyphs standard qui étend certains comportements de dessin."
type: docs
weight: 27
url: /fr/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Représente un wrapper pour les ApsGlyphs standard, qui étend une partie du comportement de dessin.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Initialise une nouvelle instance de la classe `ExtendedApsPage`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getContentSize()](#getContentSize--) | Obtient la taille de la page hors marges. |
| [getMargin()](#getMargin--) | Obtient la marge de cette page. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Obtient la position de la fin de la page, dans la page MS OneNote, lorsqu'une page MS OneNote est divisée en plusieurs pages aps. |
| [getPageSize()](#getPageSize--) | Obtient la taille finale de la page. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Obtient la position du début de la page dans la page MS OneNote, lorsqu'une page MS OneNote est divisée en plusieurs pages aps. |
| [iterator()](#iterator--) | Renvoie l'énumérateur qui parcourt tous les nœuds de cette page. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | L'énumérateur d'obtention. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Initialise une nouvelle instance de la classe `ExtendedApsPage`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | La taille de la page. |
| pageStartInNotePage | float | Le début de la page dans la page MS OneNote originale. |
| margin | com.aspose.foundation.layout.Margin | La marge de page étendue. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Obtient la taille de la page hors marges.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Obtient la marge de cette page.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Obtient la position de la fin de la page, dans la page MS OneNote, lorsqu'une page MS OneNote est divisée en plusieurs pages aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Obtient la taille finale de la page.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Obtient la position du début de la page dans la page MS OneNote, lorsqu'une page MS OneNote est divisée en plusieurs pages aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Renvoie l'énumérateur qui parcourt tous les nœuds de cette page.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Le `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


L'énumérateur d'obtention.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Le `IEnumerator`.
