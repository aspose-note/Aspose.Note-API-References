---
title: Notebook.LoadChildDocument
second_title: Aspose.Note para la referencia de la API de .NET
description: Notebook método. Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde un archivo.
type: docs
weight: 120
url: /es/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde un archivo.

```csharp
public void LoadChildDocument(string filePath)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |

### Ejemplos

Muestra cómo cargar un cuaderno desde una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Ver también

* class [Notebook](../)
* espacio de nombres [Aspose.Note](../../notebook/)
* asamblea [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde un archivo. Permite especificar opciones de carga adicionales.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |
| loadOptions | LoadOptions | Las opciones de carga. |

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* espacio de nombres [Aspose.Note](../../notebook/)
* asamblea [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde una secuencia.

```csharp
public void LoadChildDocument(Stream stream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El arroyo. |

### Ejemplos

Muestra cómo cargar un cuaderno desde una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Ver también

* class [Notebook](../)
* espacio de nombres [Aspose.Note](../../notebook/)
* asamblea [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde una secuencia. Permite especificar opciones de carga adicionales.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El arroyo. |
| loadOptions | LoadOptions | Las opciones de carga. |

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* espacio de nombres [Aspose.Note](../../notebook/)
* asamblea [Aspose.Note](../../../)


