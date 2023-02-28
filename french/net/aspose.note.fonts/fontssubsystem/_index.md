---
title: Class FontsSubsystem
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Fonts.FontsSubsystem classe. Classe de base implémentant linterface Aspose.Note.Fonts.IFontsSubsystem. Fournit des fonctionnalités pour la police par défaut et les substitutions de polices. Remplacer la fonction membre protégée Aspose.Note.Fonts.Fonts.FontsSubsystem.FetchFontFamily dans une classe dérivée pour implémenter la logique de récupération deFontFamily objet.
type: docs
weight: 110
url: /fr/net/aspose.note.fonts/fontssubsystem/
---
## FontsSubsystem class

Classe de base implémentant l'interface Aspose.Note.Fonts.IFontsSubsystem. Fournit des fonctionnalités pour la police par défaut et les substitutions de polices. Remplacer la fonction membre protégée Aspose.Note.Fonts.Fonts.FontsSubsystem.FetchFontFamily dans une classe dérivée pour implémenter la logique de récupération deFontFamily objet.

```csharp
public abstract class FontsSubsystem : IFontsSubsystem
```

## Propriétés

| Nom | La description |
| --- | --- |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Obtient ou définit la police par défaut. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont)(Stream) | Ajouter la police. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_2)(string) | Ajouter la police. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_1)(Stream, string) | Ajouter la police. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Ajoute une substitution de police. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Obtient la famille de polices. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Charge toutes les polices TrueType du dossier spécifié dans la collection interne. |

### Voir également

* interface [IFontsSubsystem](../ifontssubsystem/)
* espace de noms [Aspose.Note.Fonts](../../aspose.note.fonts/)
* Assemblée [Aspose.Note](../../)


