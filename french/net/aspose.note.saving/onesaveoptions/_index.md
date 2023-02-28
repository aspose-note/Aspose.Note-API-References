---
title: Class OneSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.OneSaveOptions classe. Permet de spécifier des options supplémentaires lors de lenregistrement dun document au format OneNote.
type: docs
weight: 810
url: /fr/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement d'un document au format OneNote.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | Obtient ou définit un mot de passe pour chiffrer le contenu du document. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Obtient ou définit les paramètres de police à utiliser lors de l'enregistrement |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. Par défaut estMaxValue ce qui signifie que toutes les pages du document seront rendues. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Obtient ou définit l'index de la première page à enregistrer. Par défaut est 0. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Obtient le format dans lequel le document est enregistré. |

### Exemples

Montre comment enregistrer un document avec cryptage.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Montre comment enregistrer un document à l'aide de OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### Voir également

* class [SaveOptions](../saveoptions/)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


