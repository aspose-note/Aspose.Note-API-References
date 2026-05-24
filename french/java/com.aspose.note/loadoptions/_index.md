---
title: "LoadOptions"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Options utilisées pour charger un document."
type: docs
weight: 46
url: /fr/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Options utilisées pour charger un document.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initialise une nouvelle instance de la classe `LoadOptions`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Obtient ou définit un mot de passe pour le contenu du document chiffré. |
| [getLoadHistory()](#getLoadHistory--) | Obtient ou définit une valeur indiquant si le chargeur de documents doit ignorer l'historique. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Obtient ou définit un mot de passe pour le contenu du document chiffré. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Obtient ou définit une valeur indiquant si le chargeur de documents doit ignorer l'historique. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialise une nouvelle instance de la classe `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Obtient ou définit un mot de passe pour le contenu du document chiffré. La valeur est ignorée si le document n'est pas protégé par un mot de passe.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Obtient ou définit une valeur indiquant si le chargeur de documents doit ignorer l'historique. Utilisez cette option pour réduire la consommation de mémoire et de CPU. La valeur par défaut est `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Obtient ou définit un mot de passe pour le contenu du document chiffré. La valeur est ignorée si le document n'est pas protégé par un mot de passe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Obtient ou définit une valeur indiquant si le chargeur de documents doit ignorer l'historique. Utilisez cette option pour réduire la consommation de mémoire et de CPU. La valeur par défaut est `true`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

