---
title: "FontsSubsystem"
second_title: "Aspose.Note for Java API-referentie"
description: "Basisklasse die de interface com.aspose.note.IFontsSubsystem implementeert."
type: docs
weight: 11
url: /nl/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Basis klasse die de interface com.aspose.note.IFontsSubsystem implementeert. Biedt functionaliteit voor het standaardlettertype en de substituties van lettertypen. Overschrijf de beschermde ledenfunctie com.aspose.note.FontsSubsystem.fetchFontFamily in een afgeleide klasse om de logica voor het ophalen van een Font-object te implementeren.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Voegt het lettertype toe. |
| [addFont(String file)](#addFont-java.lang.String-) | Voegt het lettertype toe. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Voegt lettertype-substitutie toe. |
| [getDefaultFont()](#getDefaultFont--) | Haalt het standaardlettertype op. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Haalt lettertype op. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Laadt alle TrueType-lettertypen uit de opgegeven map in de interne collectie. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Voegt het lettertype toe.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | De stroom die het lettertype bevat. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Voegt het lettertype toe.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestand | java.lang.String | Het pad naar het bestand dat het lettertype bevat. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Voegt lettertype-substitutie toe.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| vervangen | java.lang.String | De naam van het vervangen lettertype. |
| substitutie | java.lang.String | De naam van het substitutie-lettertype. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Haalt het standaardlettertype op.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Haalt lettertype op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fontName | java.lang.String | De lettertype‑naam. |

**Returns:**
java.awt.Font - Het lettertype.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Laadt alle TrueType-lettertypen uit de opgegeven map in de interne collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| map | java.lang.String | De map die lettertypen bevat. |

