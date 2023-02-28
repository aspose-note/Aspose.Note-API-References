---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note för .NET API-referens
description: OneSaveOptions fast egendom. Hämtar eller ställer in ett lösenord för att kryptera dokumentinnehållet.
type: docs
weight: 20
url: /sv/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Hämtar eller ställer in ett lösenord för att kryptera dokumentinnehållet.

```csharp
public string DocumentPassword { get; set; }
```

### Exempel

Visar hur man sparar dokument med kryptering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Se även

* class [OneSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../onesaveoptions/)
* hopsättning [Aspose.Note](../../../)


