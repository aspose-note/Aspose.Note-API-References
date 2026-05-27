---
title: "License.SetLicense"
second_title: "Aspose.Note for .NET API 参考"
description: "License 方法。为组件授权"
type: docs
weight: 20
url: /zh/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

为组件授权。

```csharp
public void SetLicense(string licenseName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| licenseName | String | 可以是完整或简短的文件名，或嵌入资源的名称。使用空字符串切换到评估模式。 |

## 备注

尝试在以下位置查找许可证：

1. 明确路径。

2. 包含 Aspose 组件程序集的文件夹。

3. 包含客户端调用程序集的文件夹。

4. 包含入口（启动）程序集的文件夹。

5. 客户端调用程序集中的嵌入资源。

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. 明确路径。

2. 客户端调用程序集中的嵌入资源。

## 示例

在此示例中，将尝试在包含组件的文件夹、包含调用程序集的文件夹、入口程序集的文件夹以及调用程序集的嵌入资源中查找名为 MyLicense.lic 的许可证文件。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

展示如何从文件加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

展示如何从嵌入的文件资源加载 Aspose.Note 的许可证。

```csharp
// 实例化 License 类
Aspose.Note.License license = new Aspose.Note.License();

// 仅传递嵌入程序集中的许可证文件名称
license.SetLicense("Aspose.Note.lic");
```

### 另请参阅

* class [License](../)
* namespace [Aspose.Note](../../license/)
* assembly [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

为组件授权。

```csharp
public void SetLicense(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 包含许可证的流。 |

## 备注

使用此方法从流加载许可证。

## 示例

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)
```

展示如何从流加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### 另请参阅

* class [License](../)
* namespace [Aspose.Note](../../license/)
* assembly [Aspose.Note](../../../)


