---
title: "NotebookLoadOptions"
second_title: "Aspose.Note for Java API-referentie"
description: "Opties die worden gebruikt om een notitieblok te laden."
type: docs
weight: 58
url: /nl/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Opties die worden gebruikt om een notitieblok te laden.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Initialiseert een nieuw exemplaar van de `NotebookLoadOptions` klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Haalt op of stelt een waarde in die aangeeft of onderliggende documenten later expliciet geladen moeten worden. |
| [getInstantLoading()](#getInstantLoading--) | Haalt op of stelt een waarde in die aangeeft of onderliggende documenten geladen moeten worden terwijl het bovenliggende document wordt geladen. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Haalt op of stelt een waarde in die aangeeft of onderliggende documenten later expliciet geladen moeten worden. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Haalt op of stelt een waarde in die aangeeft of onderliggende documenten geladen moeten worden terwijl het bovenliggende document wordt geladen. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Initialiseert een nieuw exemplaar van de `NotebookLoadOptions` klasse.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Haalt op of stelt een waarde in die aangeeft of onderliggende documenten later expliciet geladen moeten worden.

--------------------

Standaardwaarde is `false`, dus subdocumenten worden impliciet geladen. Waarde `true` geeft aan dat de gebruiker `Notebook.loadChildDocument` moet aanroepen of voor elk subknooppunt van het notitieboek nadat het notitieboek zelf is geladen. Als de waarde `true` is, wordt de optie `NotebookLoadOptions.instantLoading` genegeerd. Als het notitieboek wordt geladen vanuit een stream, is de waarde altijd `true` ondanks dat deze expliciet door de gebruiker op `false` is ingesteld.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Haalt op of stelt een waarde in die aangeeft of onderliggende documenten geladen moeten worden terwijl het bovenliggende document wordt geladen.

--------------------

Standaardwaarde is `false`, dus subdocumenten worden "lui" geladen, d.w.z. hun laden moet worden uitgesteld tot een directe toegang tot een specifiek kind. Waarde `true` geeft aan dat hun laden onmiddellijk moet gebeuren.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Haalt op of stelt een waarde in die aangeeft of onderliggende documenten later expliciet geladen moeten worden.

--------------------

Standaardwaarde is `false`, dus subdocumenten worden impliciet geladen. Waarde `true` geeft aan dat de gebruiker `Notebook.loadChildDocument` moet aanroepen of voor elk subknooppunt van het notitieboek nadat het notitieboek zelf is geladen. Als de waarde `true` is, wordt de optie `NotebookLoadOptions.instantLoading` genegeerd. Als het notitieboek wordt geladen vanuit een stream, is de waarde altijd `true` ondanks dat deze expliciet door de gebruiker op `false` is ingesteld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Haalt op of stelt een waarde in die aangeeft of onderliggende documenten geladen moeten worden terwijl het bovenliggende document wordt geladen.

--------------------

Standaardwaarde is `false`, dus subdocumenten worden "lui" geladen, d.w.z. hun laden moet worden uitgesteld tot een directe toegang tot een specifiek kind. Waarde `true` geeft aan dat hun laden onmiddellijk moet gebeuren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

