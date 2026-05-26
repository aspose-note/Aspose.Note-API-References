---
title: "NotebookSaveOptions"
second_title: "Aspose.Note for Java API-referentie"
description: "Een abstracte basisklasse die notitieblok-opslagopties voor een specifiek formaat voorstelt."
type: docs
weight: 61
url: /nl/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Een abstracte basisklasse die notitieblok-opslagopties voor een specifiek formaat voorstelt.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Haalt op of stelt een waarde in die aangeeft of kinddocumenten expliciet moeten worden opgeslagen. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Haalt de opslagopties op voor alle kinddocumenten van het notitieboek. |
| [getFlatten()](#getFlatten--) | Haalt op of stelt een waarde in die aangeeft of de hiërarchie van notebook-kinderen plat wordt opgeslagen. |
| [getSaveFormat()](#getSaveFormat--) | Haalt het formaat op waarin het notitieboek wordt opgeslagen. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Haalt op of stelt een waarde in die aangeeft of kinddocumenten expliciet moeten worden opgeslagen. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Haalt op of stelt een waarde in die aangeeft of de hiërarchie van notebook-kinderen plat wordt opgeslagen. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Haalt op of stelt een waarde in die aangeeft of kinddocumenten expliciet moeten worden opgeslagen.

--------------------

Standaardwaarde is `false`, dus subdocumenten worden impliciet opgeslagen. Waarde `true` geeft aan dat de gebruiker elk kindknooppunt van het notitieboek expliciet moet opslaan. Als het notitieboek naar een stream wordt opgeslagen, is de waarde altijd `true` ondanks dat deze expliciet door de gebruiker op `false` is ingesteld.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Haalt de opslagopties op voor alle kinddocumenten van het notitieboek.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Haalt op of stelt een waarde in die aangeeft of de hiërarchie van notebook-kinderen plat wordt opgeslagen.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Haalt het formaat op waarin het notitieboek wordt opgeslagen.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Haalt op of stelt een waarde in die aangeeft of kinddocumenten expliciet moeten worden opgeslagen.

--------------------

Standaardwaarde is `false`, dus subdocumenten worden impliciet opgeslagen. Waarde `true` geeft aan dat de gebruiker elk kindknooppunt van het notitieboek expliciet moet opslaan. Als het notitieboek naar een stream wordt opgeslagen, is de waarde altijd `true` ondanks dat deze expliciet door de gebruiker op `false` is ingesteld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Haalt op of stelt een waarde in die aangeeft of de hiërarchie van notebook-kinderen plat wordt opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

