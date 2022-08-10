---
title: Document
second_title: Référence de l'API Aspose.Note pour .NET
description: Initialise une nouvelle instance duDocumentaspose.note/document class. Crée un document OneNote vierge.
type: docs
weight: 10
url: /fr/net/aspose.note/document/document/
---
## Document() {#constructor}

Initialise une nouvelle instance du[`Document`](../../document) class. Crée un document OneNote vierge.

```csharp
public Document()
```

### Voir également

* class [Document](../../document)
* espace de noms [Aspose.Note](../../document)
* Assemblée [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Initialise une nouvelle instance du[`Document`](../../document) class. Ouvre un document OneNote existant à partir d'un fichier.

```csharp
public Document(string filePath)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Le format du document n'est pas reconnu ou n'est pas pris en charge. |
| [FileCorruptedException](../../filecorruptedexception) | Le document semble être corrompu et ne peut pas être chargé. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Le document est crypté et nécessite un mot de passe pour s'ouvrir, mais vous avez fourni un mot de passe incorrect. |
| InvalidOperationException | Il y a un problème avec le document et il doit être signalé aux développeurs Aspose.Note. |
| IOException | Il y a une exception d'entrée/sortie. |

### Voir également

* class [Document](../../document)
* espace de noms [Aspose.Note](../../document)
* Assemblée [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Initialise une nouvelle instance du[`Document`](../../document) class. Ouvre un document OneNote existant à partir d'un fichier. Permet de spécifier des options supplémentaires telles qu'un mot de passe de chiffrement.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |
| loadOptions | LoadOptions | Options utilisées pour charger un document. Peut être null. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Le format du document n'est pas reconnu ou n'est pas pris en charge. |
| [FileCorruptedException](../../filecorruptedexception) | Le document semble être corrompu et ne peut pas être chargé. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Le document est crypté et nécessite un mot de passe pour s'ouvrir, mais vous avez fourni un mot de passe incorrect. |
| InvalidOperationException | Il y a un problème avec le document et il doit être signalé aux développeurs Aspose.Note. |
| IOException | Il y a une exception d'entrée/sortie. |

### Voir également

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* espace de noms [Aspose.Note](../../document)
* Assemblée [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Initialise une nouvelle instance du[`Document`](../../document) class. Ouvre un document OneNote existant à partir d'un flux.

```csharp
public Document(Stream inStream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| inStream | Stream | Le flux. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Le format du document n'est pas reconnu ou n'est pas pris en charge. |
| [FileCorruptedException](../../filecorruptedexception) | Le document semble être corrompu et ne peut pas être chargé. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Le document est crypté et nécessite un mot de passe pour s'ouvrir, mais vous avez fourni un mot de passe incorrect. |
| InvalidOperationException | Il y a un problème avec le document et il doit être signalé aux développeurs Aspose.Note. |
| IOException | Il y a une exception d'entrée/sortie. |
| ArgumentException | Le flux ne prend pas en charge la lecture, est nul ou est déjà fermé. |

### Voir également

* class [Document](../../document)
* espace de noms [Aspose.Note](../../document)
* Assemblée [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Initialise une nouvelle instance du[`Document`](../../document) class. Ouvre un document OneNote existant à partir d'un flux. Permet de spécifier des options supplémentaires telles qu'un mot de passe de chiffrement.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| inStream | Stream | Le flux. |
| loadOptions | LoadOptions | Options utilisées pour charger un document. Peut être null. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Le format du document n'est pas reconnu ou n'est pas pris en charge. |
| [FileCorruptedException](../../filecorruptedexception) | Le document semble être corrompu et ne peut pas être chargé. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Le document est crypté et nécessite un mot de passe pour s'ouvrir, mais vous avez fourni un mot de passe incorrect. |
| InvalidOperationException | Il y a un problème avec le document et il doit être signalé aux développeurs Aspose.Note. |
| IOException | Il y a une exception d'entrée/sortie. |
| ArgumentException | Le flux ne prend pas en charge la lecture, est nul ou est déjà fermé. |

### Voir également

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* espace de noms [Aspose.Note](../../document)
* Assemblée [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
