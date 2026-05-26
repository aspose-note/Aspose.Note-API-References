---
title: "NotebookSaveOptions"
second_title: "Aspose.Note for Java API-referens"
description: "En abstrakt basklass som representerar sparalternativ för anteckningsböcker för ett specifikt format."
type: docs
weight: 61
url: /sv/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

En abstrakt basklass som representerar sparalternativ för anteckningsböcker för ett specifikt format.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Hämtar eller anger ett värde som indikerar om barn-dokument ska sparas explicit. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Hämtar sparalternativen för alla anteckningsbokens underdokument. |
| [getFlatten()](#getFlatten--) | Hämtar eller anger ett värde som indikerar om anteckningsbokens barnhierarki sparas platt. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar formatet i vilket anteckningsboken sparas. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Hämtar eller anger ett värde som indikerar om barn-dokument ska sparas explicit. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Hämtar eller anger ett värde som indikerar om anteckningsbokens barnhierarki sparas platt. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Hämtar eller anger ett värde som indikerar om barn-dokument ska sparas explicit.

--------------------

Standardvärdet är `false`, så underdokument sparas implicit. Värdet `true` indikerar att användaren bör spara varje anteckningsboks undernod explicit. Om anteckningsboken sparas till en ström är värdet alltid `true` trots att det uttryckligen sattes av användaren till `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Hämtar sparalternativen för alla anteckningsbokens underdokument.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Hämtar eller anger ett värde som indikerar om anteckningsbokens barnhierarki sparas platt.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Hämtar formatet i vilket anteckningsboken sparas.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Hämtar eller anger ett värde som indikerar om barn-dokument ska sparas explicit.

--------------------

Standardvärdet är `false`, så underdokument sparas implicit. Värdet `true` indikerar att användaren bör spara varje anteckningsboks undernod explicit. Om anteckningsboken sparas till en ström är värdet alltid `true` trots att det uttryckligen sattes av användaren till `false`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Hämtar eller anger ett värde som indikerar om anteckningsbokens barnhierarki sparas platt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

