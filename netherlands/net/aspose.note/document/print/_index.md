---
title: Document.Print
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Drukt het document af met de standaardprinter.
type: docs
weight: 130
url: /nl/net/aspose.note/document/print/
---
## Print() {#print}

Drukt het document af met de standaardprinter.

```csharp
public void Print()
```

### Voorbeelden

Laat zien hoe u een document naar een printer kunt sturen met behulp van het standaard Windows-dialoogvenster met standaardopties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Laat zien hoe u een document naar een printer kunt sturen met behulp van het standaard Windows-dialoogvenster met gespecificeerde opties.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Drukt het document af met de standaardprinter.

```csharp
public void Print(PrintOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PrintOptions | Opties die worden gebruikt om een document af te drukken. Kan nul zijn. |

### Zie ook

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


