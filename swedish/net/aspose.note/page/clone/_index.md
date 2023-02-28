---
title: Page.Clone
second_title: Aspose.Note för .NET API-referens
description: Page metod. Klonar sidan.
type: docs
weight: 140
url: /sv/net/aspose.note/page/clone/
---
## Page.Clone method

Klonar sidan.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cloneHistory | Boolean | Anger om sidans historik ska klonas.. |

### Returvärde

En klon av sidan.

### Exempel

Visar hur man överför den aktuella versionen av en sida till historiken.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Visar hur man klona en sida.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Klona till nytt dokument utan historik
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Klona till nytt dokument med historik
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Se även

* class [Page](../)
* namnutrymme [Aspose.Note](../../page/)
* hopsättning [Aspose.Note](../../../)


