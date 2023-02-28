---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note para la referencia de la API de .NET
description: LoadOptions propiedad. Obtiene o establece una contraseña para el contenido del documento cifrado. El valor se ignora en caso de que el documento no esté protegido con contraseña.
type: docs
weight: 20
url: /es/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Obtiene o establece una contraseña para el contenido del documento cifrado. El valor se ignora en caso de que el documento no esté protegido con contraseña.

```csharp
public string DocumentPassword { get; set; }
```

### Ejemplos

Muestra cómo un documento encriptado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Muestra cómo un cuaderno encriptado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Ver también

* class [LoadOptions](../)
* espacio de nombres [Aspose.Note](../../loadoptions/)
* asamblea [Aspose.Note](../../../)


