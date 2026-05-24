---
title: "SaveOptions"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Une classe de base abstraite qui représente les options d'enregistrement du document pour un format particulier."
type: docs
weight: 85
url: /fr/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Une classe de base abstraite qui représente les options d'enregistrement du document pour un format particulier.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Obtient ou définit les paramètres de la police à utiliser lors de l'enregistrement |
| [getPageCount()](#getPageCount--) | Obtient ou définit le nombre de pages à enregistrer. |
| [getPageIndex()](#getPageIndex--) | Obtient ou définit l'index de la première page à enregistrer. |
| [getSaveFormat()](#getSaveFormat--) | Obtient ou définit le format dans lequel le document est enregistré. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Obtient ou définit les paramètres de la police à utiliser lors de l'enregistrement |
| [setPageCount(int value)](#setPageCount-int-) | Obtient ou définit le nombre de pages à enregistrer. |
| [setPageIndex(int value)](#setPageIndex-int-) | Obtient ou définit l'index de la première page à enregistrer. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Obtient ou définit les paramètres de la police à utiliser lors de l'enregistrement

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtient ou définit le nombre de pages à enregistrer. Par défaut, c'est \{@link int\#Int32Extensions.MaxValue\} ce qui signifie que toutes les pages du document seront rendues.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Obtient ou définit l'index de la première page à enregistrer. Par défaut, il est 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient ou définit le format dans lequel le document est enregistré.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Obtient ou définit les paramètres de la police à utiliser lors de l'enregistrement

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Obtient ou définit le nombre de pages à enregistrer. Par défaut, c'est \{@link int\#Int32Extensions.MaxValue\} ce qui signifie que toutes les pages du document seront rendues.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Obtient ou définit l'index de la première page à enregistrer. Par défaut, il est 0.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

