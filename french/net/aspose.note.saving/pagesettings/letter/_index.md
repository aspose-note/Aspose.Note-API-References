---
title: PageSettings.Letter
second_title: Référence de l'API Aspose.Note pour .NET
description: PageSettings propriété. Récupère les paramètres de la page au format Lettre.
type: docs
weight: 30
url: /fr/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Récupère les paramètres de la page au format Lettre.

```csharp
public static PageSettings Letter { get; }
```

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

### Voir également

* class [PageSettings](../)
* espace de noms [Aspose.Note.Saving](../../pagesettings/)
* Assemblée [Aspose.Note](../../../)


