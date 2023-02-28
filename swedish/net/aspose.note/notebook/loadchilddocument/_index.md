---
title: Notebook.LoadChildDocument
second_title: Aspose.Note för .NET API-referens
description: Notebook metod. Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNotedokument från en fil.
type: docs
weight: 120
url: /sv/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en fil.

```csharp
public void LoadChildDocument(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |

### Exempel

Visar hur man laddar anteckningsboken från en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Se även

* class [Notebook](../)
* namnutrymme [Aspose.Note](../../notebook/)
* hopsättning [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en fil. Tillåter att ange ytterligare laddningsalternativ.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |
| loadOptions | LoadOptions | Inläsningsalternativen. |

### Se även

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* namnutrymme [Aspose.Note](../../notebook/)
* hopsättning [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en ström.

```csharp
public void LoadChildDocument(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Strömmen. |

### Exempel

Visar hur man laddar anteckningsboken från en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Se även

* class [Notebook](../)
* namnutrymme [Aspose.Note](../../notebook/)
* hopsättning [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

Lägger till en underordnad dokumentnod. Öppnar ett befintligt OneNote-dokument från en ström. Tillåter att ange ytterligare laddningsalternativ.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Strömmen. |
| loadOptions | LoadOptions | Inläsningsalternativen. |

### Se även

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* namnutrymme [Aspose.Note](../../notebook/)
* hopsättning [Aspose.Note](../../../)


