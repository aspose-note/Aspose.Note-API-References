---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Référence de l'API Aspose.Note pour .NET
description: DocumentFontsSubsystem méthode. Créer une nouvelle instance DocumentFontsSubsystem en utilisant une police du flux spécifié par défaut.
type: docs
weight: 50
url: /fr/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Créer une nouvelle instance DocumentFontsSubsystem en utilisant une police du flux spécifié par défaut.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| defaultFontStream | Stream | Le flux contenant le nom de la police par défaut. |
| fontsSubstitutions | Dictionary`2 | Les substitutions de polices. |

### Return_Value

Le[`DocumentFontsSubsystem`](../) .

### Exemples

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

* class [DocumentFontsSubsystem](../)
* espace de noms [Aspose.Note.Fonts](../../documentfontssubsystem/)
* Assemblée [Aspose.Note](../../../)


