---
title: Page.IsConflictPage
second_title: Aspose.Note för .NET API-referens
description: Page fast egendom. Hämtar eller ställer in ett värde som anger om den här sidan är en konfliktsida.
type: docs
weight: 50
url: /sv/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Hämtar eller ställer in ett värde som anger om den här sidan är en konfliktsida.

```csharp
public bool IsConflictPage { get; set; }
```

### Anmärkningar

Konfliktsidan uppstår när två användare försöker uppdatera samma innehåll. I det här fallet skrivs ändringarna av den första användaren som vanligt. Men ändringar av en annan användare kan inte slås samman. Så bara en kopia av sidan skapas och markerad som konflikt.

I den här versionen är konflikterna lösta till förmån för den första användarens ändringar. Så om dokumentet har konfliktsidor kommer de att visas i historiken men de kommer att hoppas över när de sparas. Det är möjligt att återställa denna flagga för att spara dessa sidor i historien som vanligt.

Detaljerat exempel på manipulering med konfliktsida finns i onlinedokumentationen.

### Exempel

Visar hur man kontrollerar om en sida är en konfliktsida (dvs. den har ändringar som OneNote inte kunde slå samman automatiskt).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument
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

    // Som standard hoppas konfliktsidor bara över när du sparar.
    // Om det markeras som icke-konflikt kommer det att sparas som vanligt i historiken.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Se även

* class [Page](../)
* namnutrymme [Aspose.Note](../../page/)
* hopsättning [Aspose.Note](../../../)


