---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note para la referencia de la API de .NET
description: OneSaveOptions propiedad. Obtiene o establece una contraseña para cifrar el contenido del documento.
type: docs
weight: 20
url: /es/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Obtiene o establece una contraseña para cifrar el contenido del documento.

```csharp
public string DocumentPassword { get; set; }
```

### Ejemplos

Muestra cómo guardar un documento con cifrado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Ver también

* class [OneSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../onesaveoptions/)
* asamblea [Aspose.Note](../../../)


