---
title: Class PageSettings
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.PageSettings classe. Représente les paramètres de mise en page dune page.
type: docs
weight: 820
url: /fr/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Représente les paramètres de mise en page d'une page.

```csharp
public class PageSettings
```

## Propriétés

| Nom | La description |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Récupère les paramètres de la page au format A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Obtient les paramètres de la page au format A4 avec une hauteur illimitée. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Récupère les paramètres de la page au format Lettre. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Obtient les paramètres de la page au format Lettre avec une hauteur illimitée. |

### Exemples

Montre comment enregistrer un document au format Pdf avec une mise en page Lettre.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Enregistre le document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Montre comment enregistrer un document au format Pdf avec une mise en page A4 sans limite de hauteur.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Enregistre le document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Voir également

* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


