---
title: "PdfSaveOptions"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages de document en PDF."
type: docs
weight: 77
url: /fr/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages de document en PDF.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initialise une nouvelle instance de la classe `PdfSaveOptions`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Obtient le type de compression appliqué aux images du fichier PDF. |
| [getJpegQuality()](#getJpegQuality--) | Obtient une valeur déterminant la qualité des images JPEG dans le document PDF. |
| [getPageSettings()](#getPageSettings--) | Obtient ou définit les paramètres de page pour chaque page du document. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Obtient ou définit l'algorithme utilisé pour le fractionnement de page. |
| [setImageCompression(int value)](#setImageCompression-int-) | Définit le type de compression appliqué aux images du fichier PDF. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Définit une valeur déterminant la qualité des images JPEG dans le document PDF. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Obtient ou définit les paramètres de page pour chaque page du document. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Obtient ou définit l'algorithme utilisé pour le fractionnement de page. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initialise une nouvelle instance de la classe `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Obtient le type de compression appliqué aux images du fichier PDF.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Obtient une valeur déterminant la qualité des images JPEG dans le document PDF. La valeur peut varier de 0 à 100 où 0 signifie la pire qualité mais une compression maximale et 100 signifie la meilleure qualité mais une compression minimale.

--------------------

La valeur par défaut est 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Obtient ou définit les paramètres de page pour chaque page du document. Par défaut, cela dépend de CurrentUICulture, \*US cultures ont le format lettre, les autres le format A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Obtient ou définit l'algorithme utilisé pour le fractionnement de page.

Valeur : le `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Définit le type de compression appliqué aux images du fichier PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Définit une valeur déterminant la qualité des images JPEG dans le document PDF. La valeur peut varier de 0 à 100 où 0 signifie la pire qualité mais une compression maximale et 100 signifie la meilleure qualité mais une compression minimale.

--------------------

La valeur par défaut est 90.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Obtient ou définit les paramètres de page pour chaque page du document. Par défaut, cela dépend de CurrentUICulture, \*US cultures ont le format lettre, les autres le format A4.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Obtient ou définit l'algorithme utilisé pour le fractionnement de page.

Valeur : le `PageSplittingAlgorithm`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

