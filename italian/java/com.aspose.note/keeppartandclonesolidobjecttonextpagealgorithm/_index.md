---
title: "KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Aggiunge la parte superiore degli oggetti alla parte inferiore della pagina e clona l'oggetto intero nella pagina successiva nel caso non si adatti nella pagina originale."
type: docs
weight: 42
url: /it/java/com.aspose.note/keeppartandclonesolidobjecttonextpagealgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm extends PageSplittingAlgorithm
```

Aggiunge la parte superiore dell'oggetto alla parte inferiore della pagina e clona l'intero oggetto nella pagina successiva nel caso in cui non si adatti nella pagina originale.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm()](#KeepPartAndCloneSolidObjectToNextPageAlgorithm--) | Inizializza una nuova istanza della classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, usando il limite di altezza predefinito della parte clonata. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)](#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-) | Inizializza una nuova istanza della classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, usando un limite di altezza specifico per la parte clonata. |
## Campi

| Campo | Descrizione |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | La dimensione massima predefinita della parte clonata. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | Ottiene il limite di altezza della parte clonata. |
### KeepPartAndCloneSolidObjectToNextPageAlgorithm() {#KeepPartAndCloneSolidObjectToNextPageAlgorithm--}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm()
```


Inizializza una nuova istanza della classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, usando il limite di altezza predefinito della parte clonata.

### KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart) {#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)
```


Inizializza una nuova istanza della classe `KeepPartAndCloneSolidObjectToNextPageAlgorithm`, usando un limite di altezza specifico per la parte clonata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| heightLimitOfClonedPart | float | L'altezza massima della parte clonata. |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


La dimensione massima predefinita della parte clonata.

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


Ottiene il limite di altezza della parte clonata.

**Returns:**
float
