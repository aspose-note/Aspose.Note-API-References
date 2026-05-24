---
title: "NotebookSaveOptionsGeneric"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Une classe de base abstraite qui représente les options d'enregistrement du carnet pour un format particulier et fournit des options d'enregistrement communes pour tous les nœuds enfants du document."
type: docs
weight: 62
url: /fr/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Une classe de base abstraite qui représente les options d'enregistrement du carnet pour un format particulier et fournit des options d'enregistrement communes pour tous les nœuds enfants du document.

`TDocumentSaveOptions` : Les options d'enregistrement pour tous les documents enfants du carnet.

TDocumentSaveOptions :
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Obtient ou définit les options d'enregistrement pour tous les documents enfants du carnet. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Obtient les options d'enregistrement pour tous les documents enfants du bloc-notes. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format dans lequel le bloc-notes est enregistré. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Obtient ou définit les options d'enregistrement pour tous les documents enfants du carnet.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Obtient les options d'enregistrement pour tous les documents enfants du bloc-notes.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format dans lequel le bloc-notes est enregistré.

**Returns:**
int
