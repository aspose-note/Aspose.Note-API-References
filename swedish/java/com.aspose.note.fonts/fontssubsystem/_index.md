---
title: "FontsSubsystem"
second_title: "Aspose.Note for Java API-referens"
description: "Bas-klass som implementerar com.aspose.note.IFontsSubsystem-gränssnittet."
type: docs
weight: 11
url: /sv/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Basisklass som implementerar com.aspose.note.IFontsSubsystem-gränssnittet. Tillhandahåller funktionalitet för standardteckensnitt och teckensnittssubstitutioner. Åsidosätt den skyddade medlemsfunktionen com.aspose.note.FontsSubsystem.fetchFontFamily i en avledd klass för att implementera logik för att hämta Font-objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Lägger till teckensnittet. |
| [addFont(String file)](#addFont-java.lang.String-) | Lägger till teckensnittet. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Lägger till teckensnittssubstitution. |
| [getDefaultFont()](#getDefaultFont--) | Hämtar standardteckensnitt. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Hämtar font. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Läser in alla TrueType-teckensnitt från angiven mapp till intern samling. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Lägger till teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen som innehåller teckensnittet. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Lägger till teckensnittet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fil | java.lang.String | Sökvägen till filen som innehåller teckensnittet. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Lägger till teckensnittssubstitution.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ersatt | java.lang.String | Namnet på det ersatta teckensnittet. |
| substitution | java.lang.String | Namnet på substitutions-teckensnittet. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Hämtar standardteckensnitt.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Hämtar font.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontName | java.lang.String | Fontnamnet. |

**Returns:**
java.awt.Font - Fonten.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Läser in alla TrueType-teckensnitt från angiven mapp till intern samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapp | java.lang.String | Mappen som innehåller teckensnitt. |

