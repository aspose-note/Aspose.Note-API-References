---
title: "NotebookSaveOptionsGeneric"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular y proporciona opciones de guardado comunes para todos los nodos hijos del documento."
type: docs
weight: 62
url: /es/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular y proporciona opciones de guardado comunes para todos los nodos hijos del documento.

`TDocumentSaveOptions`: Las opciones de guardado para todos los documentos secundarios del cuaderno.

TDocumentSaveOptions :
## Constructores

| Constructor | Descripción |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Obtiene o establece las opciones de guardado para todos los documentos secundarios del cuaderno. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Obtiene las opciones de guardado para todos los documentos hijos del cuaderno. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato en el que se guarda el cuaderno. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Obtiene o establece las opciones de guardado para todos los documentos secundarios del cuaderno.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Obtiene las opciones de guardado para todos los documentos hijos del cuaderno.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene el formato en el que se guarda el cuaderno.

**Returns:**
int
