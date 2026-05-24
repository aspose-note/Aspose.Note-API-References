---
title: "CheckBox"
second_title: "Référence d'API Aspose.Note pour Java"
description: "La classe de base pour les balises qui peuvent basculer leur état entre complet et incomplet."
type: docs
weight: 13
url: /fr/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

La classe de base pour les balises qui peuvent basculer leur état entre complet et incomplet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getChecked()](#getChecked--) | Obtient une valeur indiquant si la CheckBox est dans l'état coché. |
| [getCompletedTime()](#getCompletedTime--) | Obtient ou définit l'heure d'achèvement. |
| [getCreationTime()](#getCreationTime--) | Obtient ou définit l'heure de création. |
| [getIcon()](#getIcon--) | Obtient ou définit l'icône. |
| [getStatus()](#getStatus--) | Obtient ou définit le statut. |
| [setCompleted()](#setCompleted--) | Définit le tag à l'état terminé en utilisant l'heure actuelle comme heure de fin. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Définit le tag à l'état terminé. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Obtient ou définit l'heure de création. |
| [setOpen()](#setOpen--) | Définit l'étiquette à l'état ouvert. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Obtient une valeur indiquant si la CheckBox est dans l'état coché.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Obtient ou définit l'heure d'achèvement.

Valeur : Le `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtient ou définit l'heure de création.

Valeur : Le java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Obtient ou définit l'icône.

Valeur : Le [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Obtient ou définit le statut.

Valeur : Le [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Définit le tag à l'état terminé en utilisant l'heure actuelle comme heure de fin.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Définit le tag à l'état terminé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| completedTime | java.util.Date | L'heure de fin. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Obtient ou définit l'heure de création.

Valeur : Le java.util.Date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Définit l'étiquette à l'état ouvert.

