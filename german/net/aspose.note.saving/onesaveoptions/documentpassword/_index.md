---
title: DocumentPassword
second_title: Aspose.Note für .NET-API-Referenz
description: Ruft ein Kennwort ab oder legt es fest um den Dokumentinhalt zu verschlüsseln.
type: docs
weight: 20
url: /de/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Ruft ein Kennwort ab oder legt es fest, um den Dokumentinhalt zu verschlüsseln.

```csharp
public string DocumentPassword { get; set; }
```

### Beispiele

Zeigt, wie Dokumente verschlüsselt gespeichert werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Siehe auch

* class [OneSaveOptions](../../onesaveoptions)
* namensraum [Aspose.Note.Saving](../../onesaveoptions)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->