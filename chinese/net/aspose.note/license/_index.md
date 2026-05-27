---
title: "类 License"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.License 类。提供对组件进行授权的方法"
type: docs
weight: 370
url: /zh/net/aspose.note/license/
---
## License class

提供对组件进行授权的方法。

```csharp
public sealed class License
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [License](license/)() | 默认构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | 为组件授权。 |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | 为组件授权。 |

## 示例

在此示例中，将尝试在包含组件的文件夹、包含调用程序集的文件夹、入口程序集的文件夹以及调用程序集的嵌入资源中查找名为 MyLicense.lic 的许可证文件。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

展示如何从文件加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

展示如何从流加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

展示如何从嵌入的文件资源加载 Aspose.Note 的许可证。

```csharp
// 实例化 License 类
Aspose.Note.License license = new Aspose.Note.License();

// 仅传递嵌入程序集中的许可证文件名称
license.SetLicense("Aspose.Note.lic");
```

### 另请参阅

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


