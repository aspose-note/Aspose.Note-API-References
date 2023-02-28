---
title: SaveOptions.FontsSubsystem
second_title: Référence de l'API Aspose.Note pour .NET
description: SaveOptions propriété. Obtient ou définit les paramètres de police à utiliser lors de lenregistrement
type: docs
weight: 10
url: /fr/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

Obtient ou définit les paramètres de police à utiliser lors de l'enregistrement

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

### Exemples

Montre comment enregistrer un document au format pdf en utilisant la police par défaut spécifiée.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Montre comment enregistrer un document au format pdf en utilisant la police par défaut d'un fichier.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Montre comment enregistrer un document au format pdf en utilisant la police par défaut d'un flux.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Voir également

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* espace de noms [Aspose.Note.Saving](../../saveoptions/)
* Assemblée [Aspose.Note](../../../)


