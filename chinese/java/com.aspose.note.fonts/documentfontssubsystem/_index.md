---
title: "DocumentFontsSubsystem"
second_title: "Aspose.Note for Java API 参考"
description: "Aspose.Note.Fonts.FontsSubsystem 的简单实现。"
type: docs
weight: 10
url: /zh/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Aspose.Note.Fonts.FontsSubsystem 的简单实现。从操作系统检索 FontFamily 对象。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | 初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。 |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | 初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。 |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。 |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | 初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。 |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | 初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。 |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | 初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDefault()](#getDefault--) | 获取或设置静态默认实例。 |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | 获取或设置静态默认实例。 |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | 使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。 |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。 |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | 使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。 |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 使用指定文件中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。 |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | 使用指定流中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。 |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | 使用指定流中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。 |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 包含默认字体的流。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 字体替换。 |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 包含默认字体的流。 |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontFile | java.lang.String | 包含默认字体的文件路径。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 字体替换。 |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontFile | java.lang.String | 包含默认字体的文件路径。 |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 字体替换。 |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


初始化 [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 类的新实例。

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


获取或设置静态默认实例。

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


获取或设置静态默认实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontName | java.lang.String | 默认字体名称。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontName | java.lang.String | 默认字体名称。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 字体替换。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 包含默认字体名称的文件。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


使用指定文件中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 包含默认字体名称的文件。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 字体替换。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


使用指定流中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 包含默认字体名称的流。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


使用指定流中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 包含默认字体名称的流。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 字体替换。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
