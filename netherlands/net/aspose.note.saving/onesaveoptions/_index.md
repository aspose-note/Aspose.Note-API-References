---
title: Class OneSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.OneSaveOptions klas. Maakt het mogelijk om extra opties op te geven bij het opslaan van documenten in OneNoteindeling.
type: docs
weight: 810
url: /nl/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

Maakt het mogelijk om extra opties op te geven bij het opslaan van documenten in OneNote-indeling.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | Krijgt of stelt een wachtwoord in om de inhoud van het document te coderen. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Haalt lettertype-instellingen op of stelt deze in om te gebruiken tijdens het opslaan |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Haalt het aantal op te slaan pagina's op of stelt het in. Standaard isMaxValue wat betekent dat alle pagina's van het document worden weergegeven. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Haalt of stelt de index in van de eerste pagina die moet worden opgeslagen. Standaard is 0. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Haalt de indeling op waarin het document is opgeslagen. |

### Voorbeelden

Laat zien hoe u een document kunt opslaan met codering.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Laat zien hoe u een document kunt opslaan met behulp van OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### Zie ook

* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


