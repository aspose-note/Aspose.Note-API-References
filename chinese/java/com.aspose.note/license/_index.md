---
title: "License"
second_title: "Aspose.Note for Java API 参考"
description: "提供对组件授权的方法。"
type: docs
weight: 44
url: /zh/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

提供对组件授权的方法。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [License()](#License--) | 初始化此类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | 重置当前线程的许可证上下文。 |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | 为组件授权。 |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | 为组件授权。 |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | 为组件授权。 |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | 为当前线程设置许可证上下文。 |
### License() {#License--}
```
public License()
```


初始化此类的新实例。

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


重置当前线程的许可证上下文。

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


为组件授权。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| licenseFile | java.io.File | 许可证文件 `System.IO.FileInfo`。 |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


为组件授权。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 流 | java.io.InputStream | 包含许可证的流。 |

--------------------

`

使用此方法从流中加载许可证。

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


为组件授权。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | licenseName | java.lang.String | 可以是完整或短的文件名`或嵌入资源的名称`。使用空字符串切换到评估模式。 |

--------------------

`

尝试在以下位置查找许可证：

` `

1. 明确路径。

` `

2. 包含 Aspose 组件程序集的文件夹。

3. 包含客户端调用程序集的文件夹。

4. 包含入口（启动）程序集的文件夹。

5. 客户端调用程序集中的嵌入资源。

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. 明确路径。

2. 客户端调用程序集中的嵌入资源。

` `

2. 包含 Aspose 组件 JAR 文件的文件夹。

3. 包含客户端调用 JAR 文件的文件夹。

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


为当前线程设置许可证上下文。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 包含许可证的流。 |

