---
title: Page.Clone
second_title: Aspose.Note para la referencia de la API de .NET
description: Page método. Clona la página.
type: docs
weight: 140
url: /es/net/aspose.note/page/clone/
---
## Page.Clone method

Clona la página.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| cloneHistory | Boolean | Especifica si se debe clonar el historial de la página.. |

### Valor_devuelto

Un clon de la página.

### Ejemplos

Muestra cómo enviar la versión actual de una página al historial.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Muestra cómo clonar una página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargar documento de OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Clonar en un nuevo documento sin historial
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Clonar en un nuevo documento con historial
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Ver también

* class [Page](../)
* espacio de nombres [Aspose.Note](../../page/)
* asamblea [Aspose.Note](../../../)


