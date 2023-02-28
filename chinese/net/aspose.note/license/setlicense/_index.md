---
title: License.SetLicense
second_title: Aspose.Note for .NET API 参考
description: License 方法. 许可组件
type: docs
weight: 20
url: /zh/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

许可组件。

```csharp
public void SetLicense(string licenseName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| licenseName | String | 可以是完整或短文件名或嵌入资源的名称。 使用空字符串切换到评估模式。 |

### 评论

尝试在以下位置查找许可证：

1.显式路径。

2. 包含Aspose组件组装的文件夹。

3. 包含客户端调用程序集的文件夹。

4. 包含入口（启动）程序集的文件夹。

5. 客户端调用程序集中的嵌入式资源。

**笔记：**在 .NET Compact Framework 上，尝试仅在这些位置查找许可证：

1.显式路径。

2. 客户端调用程序集中的嵌入式资源。

### 例子

显示如何从文件加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

显示如何从嵌入式文件资源加载 Aspose.Note 的许可证。

```csharp
// 实例化许可类
Aspose.Note.License license = new Aspose.Note.License();

// 仅传递程序集中嵌入的许可证文件的名称
license.SetLicense("Aspose.Note.lic");
```

### 也可以看看

* class [License](../)
* 命名空间 [Aspose.Note](../../license/)
* 部件 [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

许可组件。

```csharp
public void SetLicense(Stream stream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 包含许可证的流。 |

### 评论

使用此方法从流中加载许可证。

### 例子

显示如何从流中加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### 也可以看看

* class [License](../)
* 命名空间 [Aspose.Note](../../license/)
* 部件 [Aspose.Note](../../../)


