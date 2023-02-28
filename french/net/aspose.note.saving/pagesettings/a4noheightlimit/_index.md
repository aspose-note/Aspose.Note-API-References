---
title: PageSettings.A4NoHeightLimit
second_title: Référence de l'API Aspose.Note pour .NET
description: PageSettings propriété. Obtient les paramètres de la page au format A4 avec une hauteur illimitée.
type: docs
weight: 20
url: /fr/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Obtient les paramètres de la page au format A4 avec une hauteur illimitée.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Exemples

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

* class [PageSettings](../)
* espace de noms [Aspose.Note.Saving](../../pagesettings/)
* Assemblée [Aspose.Note](../../../)


