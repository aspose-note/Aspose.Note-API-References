---
title: "ITag"
second_title: "Référence d'API Aspose.Note pour Java"
description: "L'interface pour les balises de toutes sortes."
type: docs
weight: 109
url: /fr/java/com.aspose.note/itag/
---
```
public interface ITag
```

L'interface pour les balises de toutes sortes.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Obtient l'heure d'achèvement. |
| [getCreationTime()](#getCreationTime--) | Obtient la date de création. |
| [getIcon()](#getIcon--) | Obtient l'icône. |
| [getLabel()](#getLabel--) | Obtient le texte du libellé. |
| [getStatus()](#getStatus--) | Obtient le statut. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Définit l'heure de création. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Obtient l'heure d'achèvement.

Valeur : Le `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Obtient la date de création.

Valeur : Le java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Obtient l'icône.

Valeur : Le [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Obtient le texte du libellé.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Obtient le statut.

Valeur : Le [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Définit l'heure de création.

Valeur : Le java.util.Date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

