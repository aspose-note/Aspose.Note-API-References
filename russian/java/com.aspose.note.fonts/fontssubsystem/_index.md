---
title: "FontsSubsystem"
second_title: "Справочник API Aspose.Note for Java"
description: "Базовый класс, реализующий интерфейс com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /ru/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Базовый класс, реализующий интерфейс com.aspose.note.IFontsSubsystem. Предоставляет функциональность для шрифта по умолчанию и его замен. Переопределите защищённую функцию‑член com.aspose.note.FontsSubsystem.fetchFontFamily в производном классе, чтобы реализовать логику получения объекта Font.
## Методы

| Метод | Описание |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Добавляет шрифт. |
| [addFont(String file)](#addFont-java.lang.String-) | Добавляет шрифт. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Добавляет замену шрифта. |
| [getDefaultFont()](#getDefaultFont--) | Получает шрифт по умолчанию. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Получает шрифт. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Загружает все TrueType шрифты из указанной папки во внутреннюю коллекцию. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Добавляет шрифт.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток, содержащий шрифт. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Добавляет шрифт.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| файл | java.lang.String | Путь к файлу, содержащему шрифт. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Добавляет замену шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| заменённый | java.lang.String | Имя заменённого шрифта. |
| замена | java.lang.String | Имя шрифта замены. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Получает шрифт по умолчанию.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Получает шрифт.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | java.lang.String | Имя шрифта. |

**Returns:**
java.awt.Font - Шрифт.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Загружает все TrueType шрифты из указанной папки во внутреннюю коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| папка | java.lang.String | Папка, содержащая шрифты. |

