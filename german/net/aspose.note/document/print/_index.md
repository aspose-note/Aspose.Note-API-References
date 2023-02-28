---
title: Document.Print
second_title: Aspose.Note für .NET-API-Referenz
description: Document methode. Druckt das Dokument mit dem Standarddrucker.
type: docs
weight: 130
url: /de/net/aspose.note/document/print/
---
## Print() {#print}

Druckt das Dokument mit dem Standarddrucker.

```csharp
public void Print()
```

### Beispiele

Zeigt, wie ein Dokument mithilfe des Standard-Windows-Dialogfelds mit Standardoptionen an einen Drucker gesendet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Zeigt, wie ein Dokument mithilfe des Windows-Standarddialogs mit festgelegten Optionen an einen Drucker gesendet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### Siehe auch

* class [Document](../)
* namensraum [Aspose.Note](../../document/)
* Montage [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Druckt das Dokument mit dem Standarddrucker.

```csharp
public void Print(PrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PrintOptions | Optionen zum Drucken eines Dokuments. Kann null sein. |

### Siehe auch

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* namensraum [Aspose.Note](../../document/)
* Montage [Aspose.Note](../../../)


