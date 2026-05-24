---
title: "FontsSubsystem"
second_title: "Aspose.Note für Java API-Referenz"
description: "Basisklasse, die das Interface com.aspose.note.IFontsSubsystem implementiert."
type: docs
weight: 11
url: /de/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Basisklasse, die das Interface com.aspose.note.IFontsSubsystem implementiert. Bietet Funktionalität für Standardschriftart und Schriftart-Substitutionen. Überschreiben Sie die geschützte Memberfunktion com.aspose.note.FontsSubsystem.fetchFontFamily in einer abgeleiteten Klasse, um die Logik zum Abrufen eines Font-Objekts zu implementieren.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Fügt die Schriftart hinzu. |
| [addFont(String file)](#addFont-java.lang.String-) | Fügt die Schriftart hinzu. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Fügt eine Schriftart-Substitution hinzu. |
| [getDefaultFont()](#getDefaultFont--) | Liefert die Standardschriftart. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Liest die Schriftart. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Lädt alle TrueType-Schriftarten aus dem angegebenen Ordner in die interne Sammlung. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Fügt die Schriftart hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Der Datenstrom, der die Schriftart enthält. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Fügt die Schriftart hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.lang.String | Der Pfad zur Datei, die die Schriftart enthält. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Fügt eine Schriftart-Substitution hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ersetzt | java.lang.String | Der Name der ersetzten Schriftart. |
| Substitution | java.lang.String | Der Name der Substitutionsschriftart. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Liefert die Standardschriftart.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Liest die Schriftart.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontName | java.lang.String | Der Schriftartname. |

**Returns:**
java.awt.Font - Die Font.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Lädt alle TrueType-Schriftarten aus dem angegebenen Ordner in die interne Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ordner | java.lang.String | Der Ordner, der Schriftarten enthält. |

