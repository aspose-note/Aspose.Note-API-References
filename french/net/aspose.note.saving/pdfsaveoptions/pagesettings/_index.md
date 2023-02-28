---
title: PdfSaveOptions.PageSettings
second_title: Référence de l'API Aspose.Note pour .NET
description: PdfSaveOptions propriété. Obtient ou définit les paramètres de page pour chaque page du document. Par défaut dépend de CurrentUICulture les cultures américaines ont un paramètre de lettre les autres ont des paramètres A4.
type: docs
weight: 40
url: /fr/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Obtient ou définit les paramètres de page pour chaque page du document. Par défaut, dépend de CurrentUICulture, *les cultures américaines ont un paramètre de lettre, les autres ont des paramètres A4.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* espace de noms [Aspose.Note.Saving](../../pdfsaveoptions/)
* Assemblée [Aspose.Note](../../../)


