---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note voor .NET API-referentie
description: OneSaveOptions eigendom. Krijgt of stelt een wachtwoord in om de inhoud van het document te coderen.
type: docs
weight: 20
url: /nl/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Krijgt of stelt een wachtwoord in om de inhoud van het document te coderen.

```csharp
public string DocumentPassword { get; set; }
```

### Voorbeelden

Laat zien hoe u een document kunt opslaan met codering.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Zie ook

* class [OneSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../onesaveoptions/)
* montage [Aspose.Note](../../../)


