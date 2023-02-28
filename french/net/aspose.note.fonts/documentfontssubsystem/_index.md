---
title: Class DocumentFontsSubsystem
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Fonts.DocumentFontsSubsystem classe. Implémentation simple de Aspose.Note.Fonts.FontsSubsystem. RécupèreFontFamily objet du système dexploitation.
type: docs
weight: 100
url: /fr/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Implémentation simple de Aspose.Note.Fonts.FontsSubsystem. RécupèreFontFamily objet du système d'exploitation.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Initialise une nouvelle instance du`DocumentFontsSubsystem` classe. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Initialise une nouvelle instance du`DocumentFontsSubsystem` classe. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Initialise une nouvelle instance du`DocumentFontsSubsystem` classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Obtient ou définit l'instance statique par défaut. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Obtient ou définit la police par défaut. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Créer une nouvelle instance DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Créer une nouvelle instance DocumentFontsSubsystem en utilisant une police du fichier spécifié par défaut. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Créer une nouvelle instance DocumentFontsSubsystem en utilisant une police du flux spécifié par défaut. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Ajouter la police. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Ajouter la police. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Ajouter la police. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Ajoute une substitution de police. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Obtient la famille de polices. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Charge toutes les polices TrueType du dossier spécifié dans la collection interne. |

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

* class [FontsSubsystem](../fontssubsystem/)
* espace de noms [Aspose.Note.Fonts](../../aspose.note.fonts/)
* Assemblée [Aspose.Note](../../)


