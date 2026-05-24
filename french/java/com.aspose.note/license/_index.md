---
title: "License"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Fournit des méthodes pour licencier le composant."
type: docs
weight: 44
url: /fr/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Fournit des méthodes pour licencier le composant.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [License()](#License--) | Initialise une nouvelle instance de cette classe. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Réinitialise le contexte de licence pour le thread actuel. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licence le composant. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licence le composant. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licence le composant. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Définit un contexte de licence pour le thread actuel. |
### License() {#License--}
```
public License()
```


Initialise une nouvelle instance de cette classe.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Réinitialise le contexte de licence pour le thread actuel.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licence le composant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| licenseFile | java.io.File | Fichier de licence `System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licence le composant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | flux | java.io.InputStream | Un flux qui contient la licence. |

--------------------

`

Utilisez cette méthode pour charger une licence à partir d'un flux.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licence le composant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | licenseName | java.lang.String | Peut être un nom de fichier complet ou court` or name of an embedded resource`. Utilisez une chaîne vide pour passer en mode d'évaluation. |

--------------------

`

Essaie de trouver la licence aux emplacements suivants :

` `

1. Chemin explicite.

` `

2. Le dossier qui contient l'assembly du composant Aspose.

3. Le dossier qui contient l'assembly appelant du client.

4. Le dossier qui contient l'assembly d'entrée (démarrage).

5. Une ressource intégrée dans l'assembly appelant du client.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Chemin explicite.

2. Une ressource intégrée dans l'assembly appelant du client.

` `

2. Le dossier qui contient le fichier JAR du composant Aspose.

3. Le dossier qui contient le fichier JAR appelant du client.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Définit un contexte de licence pour le thread actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Un flux qui contient la licence. |

