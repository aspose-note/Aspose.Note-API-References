---
title: Page.IsConflictPage
second_title: Aspose.Note für .NET-API-Referenz
description: Page eigendom. Ruft einen Wert ab oder legt einen Wert fest der angibt ob diese Seite eine Konfliktseite ist.
type: docs
weight: 50
url: /de/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob diese Seite eine Konfliktseite ist.

```csharp
public bool IsConflictPage { get; set; }
```

### Bemerkungen

Die Konfliktseite entsteht, wenn zwei Benutzer versuchen, denselben Inhalt zu aktualisieren. In diesem Fall werden die Änderungen des ersten Benutzers wie gewohnt geschrieben. Änderungen eines anderen Benutzers können jedoch nicht zusammengeführt werden. Es wird also nur eine Kopie der Seite erstellt und als Konflikt markiert.

In dieser Version werden die Konflikte zugunsten der Änderungen des ersten Benutzers gelöst. Wenn also ein Dokument Konfliktseiten hat, werden sie im Verlauf angezeigt, aber beim Speichern übersprungen. Es ist möglich, dieses Flag zurückzusetzen, um diese Seiten zu speichern in der Geschichte wie gewohnt.

Ein detailliertes Beispiel für die Manipulation von Konfliktseiten finden Sie in der Online-Dokumentation.

### Beispiele

Zeigt, wie überprüft wird, ob es sich bei einer Seite um eine Konfliktseite handelt (d. h. sie enthält Änderungen, die OneNote nicht automatisch zusammenführen konnte).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Standardmäßig werden Konfliktseiten beim Speichern einfach übersprungen.
    // Wenn es als Nicht-Konflikt markiert wird, wird es wie gewohnt im Verlauf gespeichert.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Siehe auch

* class [Page](../)
* namensraum [Aspose.Note](../../page/)
* Montage [Aspose.Note](../../../)


