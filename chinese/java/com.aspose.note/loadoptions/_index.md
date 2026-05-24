---
title: "LoadOptions"
second_title: "Aspose.Note for Java API 参考"
description: "用于加载文档的选项。"
type: docs
weight: 46
url: /zh/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

用于加载文档的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | 初始化 `LoadOptions` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | 获取或设置加密文档内容的密码。 |
| [getLoadHistory()](#getLoadHistory--) | 获取或设置一个值，指示文档加载器是否应忽略历史记录。 |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | 获取或设置加密文档内容的密码。 |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | 获取或设置一个值，指示文档加载器是否应忽略历史记录。 |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


初始化 `LoadOptions` 类的新实例。

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


获取或设置加密文档内容的密码。如果文档未受密码保护，则该值将被忽略。

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


获取或设置一个值，指示文档加载器是否应忽略历史记录。使用此选项可降低内存和 CPU 使用率。默认值为 `true`。

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


获取或设置加密文档内容的密码。如果文档未受密码保护，则该值将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


获取或设置一个值，指示文档加载器是否应忽略历史记录。使用此选项可降低内存和 CPU 使用率。默认值为 `true`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

