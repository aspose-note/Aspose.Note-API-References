---
title: Document.Document
second_title: Aspose.Note for .NET API 参考
description: Document 构造函数. 初始化一个新的实例Document class. 创建一个空白的 OneNote 文档
type: docs
weight: 10
url: /zh/net/aspose.note/document/document/
---
## Document() {#constructor}

初始化一个新的实例[`Document`](../) class. 创建一个空白的 OneNote 文档。

```csharp
public Document()
```

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

初始化一个新的实例[`Document`](../) class. 从文件中打开现有的 OneNote 文档。

```csharp
public Document(string filePath)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 文档格式无法识别或不受支持。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 该文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档有问题，应该报告给 Aspose.Note 开发人员。 |
| IOException | 存在输入/输出异常。 |

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

初始化一个新的实例[`Document`](../)class. 从文件中打开现有的 OneNote 文档。允许指定其他选项，例如加密密码。

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| loadOptions | LoadOptions | 用于加载文档的选项。可以为 null. |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 文档格式无法识别或不受支持。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 该文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档有问题，应该报告给 Aspose.Note 开发人员。 |
| IOException | 存在输入/输出异常。 |

### 也可以看看

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

初始化一个新的实例[`Document`](../) class. 从流中打开现有的 OneNote 文档。

```csharp
public Document(Stream inStream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| inStream | Stream | 流. |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 文档格式无法识别或不受支持。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 该文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档有问题，应该报告给 Aspose.Note 开发人员。 |
| IOException | 存在输入/输出异常。 |
| ArgumentException | 流不支持读取、为空或已关闭。 |

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

初始化一个新的实例[`Document`](../) class. 从流中打开现有的 OneNote 文档。允许指定其他选项，例如加密密码。

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| inStream | Stream | 流. |
| loadOptions | LoadOptions | 用于加载文档的选项。可以为 null. |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 文档格式无法识别或不受支持。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 该文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档有问题，应该报告给 Aspose.Note 开发人员。 |
| IOException | 存在输入/输出异常。 |
| ArgumentException | 流不支持读取、为空或已关闭。 |

### 也可以看看

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


