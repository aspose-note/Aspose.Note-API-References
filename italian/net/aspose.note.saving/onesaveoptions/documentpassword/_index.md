---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note per .NET API Reference
description: OneSaveOptions proprietà. Ottiene o imposta una password per crittografare il contenuto del documento.
type: docs
weight: 20
url: /it/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Ottiene o imposta una password per crittografare il contenuto del documento.

```csharp
public string DocumentPassword { get; set; }
```

### Esempi

Mostra come salvare il documento con crittografia.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Guarda anche

* class [OneSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../onesaveoptions/)
* assemblea [Aspose.Note](../../../)


