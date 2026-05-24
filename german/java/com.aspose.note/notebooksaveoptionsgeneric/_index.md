---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note für Java API-Referenz"
description: "Eine abstrakte Basisklasse, die Notizbuch-Speicheroptionen für ein bestimmtes Format darstellt und gemeinsame Speicheroptionen für alle untergeordneten Dokumentknoten bereitstellt."
type: docs
weight: 62
url: /de/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Eine abstrakte Basisklasse, die Notizbuch-Speicheroptionen für ein bestimmtes Format darstellt und gemeinsame Speicheroptionen für alle untergeordneten Dokumentknoten bereitstellt.

`TDocumentSaveOptions`: Die Speicheroptionen für alle Unterdokumente des Notizbuchs.

TDocumentSaveOptions :
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Liest oder setzt die Speicheroptionen für alle Unterdokumente des Notizbuchs. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Ermittelt die Speicheroptionen für alle Kinddokumente des Notizbuchs. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Format, in dem das Notizbuch gespeichert wird. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Liest oder setzt die Speicheroptionen für alle Unterdokumente des Notizbuchs.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Ermittelt die Speicheroptionen für alle Kinddokumente des Notizbuchs.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ermittelt das Format, in dem das Notizbuch gespeichert wird.

**Returns:**
int
