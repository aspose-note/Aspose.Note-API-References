---
title: Document.Print
second_title: Référence de l'API Aspose.Note pour .NET
description: Document méthode. Imprime le document à laide de limprimante par défaut.
type: docs
weight: 130
url: /fr/net/aspose.note/document/print/
---
## Print() {#print}

Imprime le document à l'aide de l'imprimante par défaut.

```csharp
public void Print()
```

### Exemples

Montre comment envoyer un document à une imprimante à l'aide de la boîte de dialogue Windows standard avec les options par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Montre comment envoyer un document à une imprimante à l'aide de la boîte de dialogue Windows standard avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Imprime le document à l'aide de l'imprimante par défaut.

```csharp
public void Print(PrintOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| options | PrintOptions | Options utilisées pour imprimer un document. Peut être null. |

### Voir également

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


