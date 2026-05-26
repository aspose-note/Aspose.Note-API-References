---
title: "FontsSubsystem"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Clase base que implementa la interfaz com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /es/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Clase base que implementa la interfaz com.aspose.note.IFontsSubsystem. Proporciona funcionalidad para la fuente predeterminada y las sustituciones de fuentes. Anule la función de miembro protegido com.aspose.note.FontsSubsystem.fetchFontFamily en una clase derivada para implementar la lógica de recuperación del objeto Font.
## Métodos

| Método | Descripción |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Agrega la fuente. |
| [addFont(String file)](#addFont-java.lang.String-) | Agrega la fuente. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Agrega sustitución de fuente. |
| [getDefaultFont()](#getDefaultFont--) | Obtiene la fuente predeterminada. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Obtiene la fuente. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Carga todas las fuentes TrueType de la carpeta especificada a la colección interna. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Agrega la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo que contiene la fuente. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Agrega la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivo | java.lang.String | La ruta al archivo que contiene la fuente. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Agrega sustitución de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sustituida | java.lang.String | El nombre de la fuente sustituida. |
| sustitución | java.lang.String | El nombre de la fuente de sustitución. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Obtiene la fuente predeterminada.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Obtiene la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontName | java.lang.String | El nombre de la fuente. |

**Returns:**
java.awt.Font - La Font.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Carga todas las fuentes TrueType de la carpeta especificada a la colección interna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| carpeta | java.lang.String | La carpeta que contiene fuentes. |

