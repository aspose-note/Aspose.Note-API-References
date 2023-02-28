---
title: Page.Clone
second_title: Aspose.Note für .NET-API-Referenz
description: Page methode. Klont die Seite.
type: docs
weight: 140
url: /de/net/aspose.note/page/clone/
---
## Page.Clone method

Klont die Seite.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cloneHistory | Boolean | Gibt an, ob der Seitenverlauf geklont werden soll.. |

### Rückgabewert

Ein Klon der Seite.

### Beispiele

Zeigt, wie die aktuelle Version einer Seite in den Verlauf verschoben wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden und erstes untergeordnetes Element abrufen           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Zeigt, wie eine Seite geklont wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// In neues Dokument ohne Historie klonen
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// In neues Dokument mit Verlauf klonen
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Siehe auch

* class [Page](../)
* namensraum [Aspose.Note](../../page/)
* Montage [Aspose.Note](../../../)


