---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Référence de l'API Aspose.Note pour .NET
description: DocumentFontsSubsystem méthode. Créer une nouvelle instance DocumentFontsSubsystem en utilisant une police du fichier spécifié par défaut.
type: docs
weight: 40
url: /fr/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Créer une nouvelle instance DocumentFontsSubsystem en utilisant une police du fichier spécifié par défaut.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le fichier contenant le nom de la police par défaut. |
| fontsSubstitutions | Dictionary`2 | Les substitutions de polices. |

### Return_Value

Le[`DocumentFontsSubsystem`](../) .

### Exemples

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

### Voir également

* class [DocumentFontsSubsystem](../)
* espace de noms [Aspose.Note.Fonts](../../documentfontssubsystem/)
* Assemblée [Aspose.Note](../../../)


