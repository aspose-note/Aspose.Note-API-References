---
title: "NotebookLoadOptions"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Options utilisées pour charger un carnet."
type: docs
weight: 58
url: /fr/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Options utilisées pour charger un carnet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Initialise une nouvelle instance de la classe `NotebookLoadOptions` . |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés explicitement plus tard. |
| [getInstantLoading()](#getInstantLoading--) | Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés pendant le chargement du document parent. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés explicitement plus tard. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés pendant le chargement du document parent. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Initialise une nouvelle instance de la classe `NotebookLoadOptions` .

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés explicitement plus tard.

--------------------

La valeur par défaut est `false`, donc les documents enfants seront chargés implicitement. La valeur `true` indique que l'utilisateur doit appeler `Notebook.loadChildDocument` ou pour chaque nœud enfant du carnet après que le carnet lui‑même soit chargé. Si la valeur est `true`, l'option `NotebookLoadOptions.instantLoading` sera ignorée. Si le carnet est chargé depuis un flux, la valeur est toujours `true` même si l'utilisateur l'a explicitement définie sur `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés pendant le chargement du document parent.

--------------------

La valeur par défaut est `false`, donc les documents enfants seront chargés paresseusement, c’est‑à‑dire que leur chargement doit être différé jusqu’à un accès direct à l’enfant spécifique. La valeur `true` indique que leur chargement doit être effectué immédiatement.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés explicitement plus tard.

--------------------

La valeur par défaut est `false`, donc les documents enfants seront chargés implicitement. La valeur `true` indique que l'utilisateur doit appeler `Notebook.loadChildDocument` ou pour chaque nœud enfant du carnet après que le carnet lui‑même soit chargé. Si la valeur est `true`, l'option `NotebookLoadOptions.instantLoading` sera ignorée. Si le carnet est chargé depuis un flux, la valeur est toujours `true` même si l'utilisateur l'a explicitement définie sur `false`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Obtient ou définit une valeur indiquant si les documents enfants doivent être chargés pendant le chargement du document parent.

--------------------

La valeur par défaut est `false`, donc les documents enfants seront chargés paresseusement, c’est‑à‑dire que leur chargement doit être différé jusqu’à un accès direct à l’enfant spécifique. La valeur `true` indique que leur chargement doit être effectué immédiatement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

