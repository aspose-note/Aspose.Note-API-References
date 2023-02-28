---
title: Notebook.LoadChildDocument
second_title: Aspose.Note voor .NET API-referentie
description: Notebook methode. Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNotedocument vanuit een bestand.
type: docs
weight: 120
url: /nl/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document vanuit een bestand.

```csharp
public void LoadChildDocument(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |

### Voorbeelden

Laat zien hoe je een notebook laadt vanuit een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Zie ook

* class [Notebook](../)
* naamruimte [Aspose.Note](../../notebook/)
* montage [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document vanuit een bestand. Maakt het mogelijk om extra laadopties te specificeren.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |
| loadOptions | LoadOptions | De laadopties. |

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* naamruimte [Aspose.Note](../../notebook/)
* montage [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document uit een stream.

```csharp
public void LoadChildDocument(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom. |

### Voorbeelden

Laat zien hoe je een notebook laadt vanuit een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Zie ook

* class [Notebook](../)
* naamruimte [Aspose.Note](../../notebook/)
* montage [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

Voegt een onderliggend documentknooppunt toe. Opent een bestaand OneNote-document uit een stroom. Maakt het mogelijk om extra laadopties te specificeren.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom. |
| loadOptions | LoadOptions | De laadopties. |

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* naamruimte [Aspose.Note](../../notebook/)
* montage [Aspose.Note](../../../)


