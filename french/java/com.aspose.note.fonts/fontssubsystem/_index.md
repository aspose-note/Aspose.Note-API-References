---
title: "FontsSubsystem"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Classe de base implémentant l'interface com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /fr/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Classe de base implémentant l'interface com.aspose.note.IFontsSubsystem. Fournit des fonctionnalités pour la police par défaut et les substitutions de police. Surchargez la fonction membre protégée com.aspose.note.FontsSubsystem.fetchFontFamily dans une classe dérivée pour implémenter la logique de récupération de l'objet Font.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Ajoute la police. |
| [addFont(String file)](#addFont-java.lang.String-) | Ajoute la police. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Ajoute une substitution de police. |
| [getDefaultFont()](#getDefaultFont--) | Obtient la police par défaut. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Obtient la police. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Charge toutes les polices TrueType du dossier spécifié dans la collection interne. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Ajoute la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux contenant la police. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Ajoute la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fichier | java.lang.String | Le chemin vers le fichier contenant la police. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Ajoute une substitution de police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| substituée | java.lang.String | Le nom de la police substituée. |
| substitution | java.lang.String | Le nom de la police de substitution. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Obtient la police par défaut.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Obtient la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | Le nom de la police. |

**Returns:**
java.awt.Font - La police.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Charge toutes les polices TrueType du dossier spécifié dans la collection interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dossier | java.lang.String | Le dossier contenant les polices. |

