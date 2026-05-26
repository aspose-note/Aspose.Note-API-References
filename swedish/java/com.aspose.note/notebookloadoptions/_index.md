---
title: "NotebookLoadOptions"
second_title: "Aspose.Note for Java API-referens"
description: "Alternativ som används för att läsa in en anteckningsbok."
type: docs
weight: 58
url: /sv/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Alternativ som används för att läsa in en anteckningsbok.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Initierar en ny instans av klassen `NotebookLoadOptions`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Hämtar eller anger ett värde som indikerar om underdokument ska laddas explicit senare. |
| [getInstantLoading()](#getInstantLoading--) | Hämtar eller anger ett värde som indikerar om underdokument ska laddas medan förälderdokumentet laddas. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Hämtar eller anger ett värde som indikerar om underdokument ska laddas explicit senare. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Hämtar eller anger ett värde som indikerar om underdokument ska laddas medan förälderdokumentet laddas. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Initierar en ny instans av klassen `NotebookLoadOptions`.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Hämtar eller anger ett värde som indikerar om underdokument ska laddas explicit senare.

--------------------

Standardvärdet är `false`, så underdokument laddas implicit. Värdet `true` indikerar att användaren bör anropa `Notebook.loadChildDocument` eller för varje notebooks undernod efter att själva notebook har laddats. Om värdet är `true` kommer alternativet `NotebookLoadOptions.instantLoading` att ignoreras. Om notebook laddas från en ström är värdet alltid `true` trots att det uttryckligen satts av användaren till `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Hämtar eller anger ett värde som indikerar om underdokument ska laddas medan förälderdokumentet laddas.

--------------------

Standardvärdet är `false`, så underdokument kommer att laddas \"lazily\", d.v.s. deras laddning bör skjutas upp tills en direkt åtkomst till ett specifikt underdokument. Värdet `true` indikerar att deras laddning ska göras omedelbart.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Hämtar eller anger ett värde som indikerar om underdokument ska laddas explicit senare.

--------------------

Standardvärdet är `false`, så underdokument laddas implicit. Värdet `true` indikerar att användaren bör anropa `Notebook.loadChildDocument` eller för varje notebooks undernod efter att själva notebook har laddats. Om värdet är `true` kommer alternativet `NotebookLoadOptions.instantLoading` att ignoreras. Om notebook laddas från en ström är värdet alltid `true` trots att det uttryckligen satts av användaren till `false`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Hämtar eller anger ett värde som indikerar om underdokument ska laddas medan förälderdokumentet laddas.

--------------------

Standardvärdet är `false`, så underdokument kommer att laddas \"lazily\", d.v.s. deras laddning bör skjutas upp tills en direkt åtkomst till ett specifikt underdokument. Värdet `true` indikerar att deras laddning ska göras omedelbart.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

