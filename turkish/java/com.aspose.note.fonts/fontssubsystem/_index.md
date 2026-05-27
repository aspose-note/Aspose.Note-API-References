---
title: "FontsSubsystem"
second_title: "Aspose.Note for Java API Referansı"
description: "com.aspose.note.IFontsSubsystem arabirimini uygulayan temel sınıf."
type: docs
weight: 11
url: /tr/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

com.aspose.note.IFontsSubsystem arayüzünü uygulayan temel sınıf. Varsayılan yazı tipi ve yazı tipi ikameleri için işlevsellik sağlar. Font nesnesini elde etmek için mantığı uygulamak amacıyla türetilmiş bir sınıfta com.aspose.note.FontsSubsystem.fetchFontFamily korumalı üye işlevini geçersiz kılın.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Yazı tipini ekler. |
| [addFont(String file)](#addFont-java.lang.String-) | Yazı tipini ekler. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Yazı tipi ikamesi ekler. |
| [getDefaultFont()](#getDefaultFont--) | Varsayılan yazı tipini alır. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Yazı tipini alır. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Belirtilen klasörden tüm TrueType yazı tiplerini iç koleksiyona yükler. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Yazı tipini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Yazı tipini içeren akış. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Yazı tipini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.lang.String | Yazı tipini içeren dosyanın yolu. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Yazı tipi ikamesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ikame edilen | java.lang.String | İkame edilen yazı tipi adı. |
| ikame | java.lang.String | İkame yazı tipi adı. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Varsayılan yazı tipini alır.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Yazı tipini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontName | java.lang.String | Yazı tipi adı. |

**Returns:**
java.awt.Font - Font.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Belirtilen klasörden tüm TrueType yazı tiplerini iç koleksiyona yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| klasör | java.lang.String | Yazı tiplerini içeren klasör. |

