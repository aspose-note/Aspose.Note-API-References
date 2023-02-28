---
title: Page.Clone
second_title: Aspose.Note voor .NET API-referentie
description: Page methode. Kloont de pagina.
type: docs
weight: 140
url: /nl/net/aspose.note/page/clone/
---
## Page.Clone method

Kloont de pagina.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cloneHistory | Boolean | Geeft aan of de geschiedenis van de pagina moet worden gekloond.. |

### Winstwaarde

Een kloon van de pagina.

### Voorbeelden

Laat zien hoe de huidige versie van een pagina naar de geschiedenis kan worden gepusht.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Laat zien hoe u een pagina kunt klonen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Kloon in een nieuw document zonder geschiedenis
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Kloon in een nieuw document met geschiedenis
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Zie ook

* class [Page](../)
* naamruimte [Aspose.Note](../../page/)
* montage [Aspose.Note](../../../)


