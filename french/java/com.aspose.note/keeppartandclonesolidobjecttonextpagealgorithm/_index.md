---
title: "KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Ajoute la partie supérieure des objets au bas de la page et clone l'objet complet vers la page suivante au cas où il ne tiendrait pas dans la page d'origine."
type: docs
weight: 42
url: /fr/java/com.aspose.note/keeppartandclonesolidobjecttonextpagealgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm extends PageSplittingAlgorithm
```

Ajoute la partie supérieure de l'objet au bas de la page et clone l'objet complet sur la page suivante au cas où il ne tiendrait pas dans la page d'origine.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm()](#KeepPartAndCloneSolidObjectToNextPageAlgorithm--) | Initialise une nouvelle instance de la classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, en utilisant la limite de hauteur par défaut de la partie clonée. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)](#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-) | Initialise une nouvelle instance de la classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, en utilisant une limite de hauteur spécifique pour la partie clonée. |
## Champs

| Champ | Description |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | La taille maximale par défaut de la partie clonée. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | Obtient la limite de hauteur de la partie clonée. |
### KeepPartAndCloneSolidObjectToNextPageAlgorithm() {#KeepPartAndCloneSolidObjectToNextPageAlgorithm--}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm()
```


Initialise une nouvelle instance de la classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, en utilisant la limite de hauteur par défaut de la partie clonée.

### KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart) {#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)
```


Initialise une nouvelle instance de la classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, en utilisant une limite de hauteur spécifique pour la partie clonée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| heightLimitOfClonedPart | float | La hauteur maximale de la partie clonée. |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


La taille maximale par défaut de la partie clonée.

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


Obtient la limite de hauteur de la partie clonée.

**Returns:**
float
