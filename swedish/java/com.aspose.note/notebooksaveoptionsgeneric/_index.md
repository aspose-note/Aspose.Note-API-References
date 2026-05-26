---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note for Java API-referens"
description: "En abstrakt basklass som representerar sparalternativ för anteckningsböcker för ett specifikt format och tillhandahåller gemensamma sparalternativ för alla underordnade dokumentnoder."
type: docs
weight: 62
url: /sv/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

En abstrakt basklass som representerar sparalternativ för anteckningsböcker för ett specifikt format och tillhandahåller gemensamma sparalternativ för alla underordnade dokumentnoder.

`TDocumentSaveOptions`: Sparaalternativen för alla underdokument i anteckningsboken.

TDocumentSaveOptions :
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Hämtar eller anger sparaalternativen för alla underdokument i anteckningsboken. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Hämtar sparalternativen för alla anteckningsbokens underdokument. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar formatet i vilket anteckningsboken sparas. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Hämtar eller anger sparaalternativen för alla underdokument i anteckningsboken.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Hämtar sparalternativen för alla anteckningsbokens underdokument.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar formatet i vilket anteckningsboken sparas.

**Returns:**
int
