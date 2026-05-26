---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note for Java API-referentie"
description: "Een abstracte basisklasse die notitieblok-opslagopties voor een specifiek formaat voorstelt en gemeenschappelijke opslagopties biedt voor alle onderliggende knooppunten van het document."
type: docs
weight: 62
url: /nl/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Een abstracte basisklasse die notitieblok-opslagopties voor een specifiek formaat voorstelt en gemeenschappelijke opslagopties biedt voor alle onderliggende knooppunten van het document.

`TDocumentSaveOptions`: De opslagopties voor alle onderliggende documenten van het notitieboek.

TDocumentSaveOptions :
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Haalt of stelt de opslagopties in voor alle onderliggende documenten van het notitieboek. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Haalt de opslagopties op voor alle kinddocumenten van het notitieboek. |
| [getSaveFormat()](#getSaveFormat--) | Haalt het formaat op waarin het notitieboek wordt opgeslagen. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Haalt of stelt de opslagopties in voor alle onderliggende documenten van het notitieboek.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Haalt de opslagopties op voor alle kinddocumenten van het notitieboek.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Haalt het formaat op waarin het notitieboek wordt opgeslagen.

**Returns:**
int
