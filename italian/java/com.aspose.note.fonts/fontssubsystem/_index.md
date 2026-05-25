---
title: "FontsSubsystem"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Classe base che implementa l'interfaccia com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /it/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Classe base che implementa l'interfaccia com.aspose.note.IFontsSubsystem. Fornisce funzionalità per il font predefinito e le sostituzioni dei font. Sovrascrivi la funzione membro protetta com.aspose.note.FontsSubsystem.fetchFontFamily in una classe derivata per implementare la logica di recupero dell'oggetto Font.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Aggiunge il font. |
| [addFont(String file)](#addFont-java.lang.String-) | Aggiunge il font. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Aggiunge la sostituzione del font. |
| [getDefaultFont()](#getDefaultFont--) | Ottiene il font predefinito. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Ottiene il font. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Carica tutti i font TrueType dalla cartella specificata nella collezione interna. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Aggiunge il font.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Il flusso che contiene il font. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Aggiunge il font.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.lang.String | Il percorso del file che contiene il font. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Aggiunge la sostituzione del font.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sostituito | java.lang.String | Il nome del font sostituito. |
| sostituzione | java.lang.String | Il nome del font di sostituzione. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Ottiene il font predefinito.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Ottiene il font.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontName | java.lang.String | Il nome del font. |

**Returns:**
java.awt.Font - Il Font.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Carica tutti i font TrueType dalla cartella specificata nella collezione interna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cartella | java.lang.String | La cartella che contiene i font. |

