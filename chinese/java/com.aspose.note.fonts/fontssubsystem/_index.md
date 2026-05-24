---
title: "FontsSubsystem"
second_title: "Aspose.Note for Java API 参考"
description: "实现 com.aspose.note.IFontsSubsystem 接口的基类。"
type: docs
weight: 11
url: /zh/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

实现 com.aspose.note.IFontsSubsystem 接口的基类。提供默认字体和字体替换的功能。覆盖派生类中的 com.aspose.note.FontsSubsystem.fetchFontFamily 受保护成员函数，以实现检索 Font 对象的逻辑。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | 添加字体。 |
| [addFont(String file)](#addFont-java.lang.String-) | 添加字体。 |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | 添加字体替换。 |
| [getDefaultFont()](#getDefaultFont--) | 获取默认字体。 |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | 获取字体。 |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | 从指定文件夹加载所有 TrueType 字体到内部集合。 |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


添加字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 包含字体的流。 |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


添加字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | java.lang.String | 包含字体的文件路径。 |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


添加字体替换。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 已替换 | java.lang.String | 已替换的字体名称。 |
| 替换 | java.lang.String | 替换字体名称。 |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


获取默认字体。

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


获取字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontName | java.lang.String | 字体名称。 |

**Returns:**
java.awt.Font - 字体。
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


从指定文件夹加载所有 TrueType 字体到内部集合。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件夹 | java.lang.String | 包含字体的文件夹。 |

