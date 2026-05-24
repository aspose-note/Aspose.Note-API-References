---
title: "NotebookSaveOptions"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Une classe de base abstraite qui représente les options d'enregistrement du carnet pour un format particulier."
type: docs
weight: 61
url: /fr/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Une classe de base abstraite qui représente les options d'enregistrement du carnet pour un format particulier.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Obtient ou définit une valeur indiquant si les documents enfants doivent être enregistrés explicitement. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Obtient les options d'enregistrement pour tous les documents enfants du bloc-notes. |
| [getFlatten()](#getFlatten--) | Obtient ou définit une valeur indiquant si la hiérarchie des enfants du bloc-notes est enregistrée à plat. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format dans lequel le bloc-notes est enregistré. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Obtient ou définit une valeur indiquant si les documents enfants doivent être enregistrés explicitement. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Obtient ou définit une valeur indiquant si la hiérarchie des enfants du bloc-notes est enregistrée à plat. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Obtient ou définit une valeur indiquant si les documents enfants doivent être enregistrés explicitement.

--------------------

La valeur par défaut est `false`, donc les documents enfants seront enregistrés implicitement. La valeur `true` indique que l'utilisateur doit enregistrer chaque nœud enfant du carnet explicitement. Si le carnet est enregistré dans un flux, la valeur est toujours `true` même si l'utilisateur l'a explicitement définie sur `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Obtient les options d'enregistrement pour tous les documents enfants du bloc-notes.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Obtient ou définit une valeur indiquant si la hiérarchie des enfants du bloc-notes est enregistrée à plat.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Obtient le format dans lequel le bloc-notes est enregistré.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Obtient ou définit une valeur indiquant si les documents enfants doivent être enregistrés explicitement.

--------------------

La valeur par défaut est `false`, donc les documents enfants seront enregistrés implicitement. La valeur `true` indique que l'utilisateur doit enregistrer chaque nœud enfant du carnet explicitement. Si le carnet est enregistré dans un flux, la valeur est toujours `true` même si l'utilisateur l'a explicitement définie sur `false`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Obtient ou définit une valeur indiquant si la hiérarchie des enfants du bloc-notes est enregistrée à plat.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

