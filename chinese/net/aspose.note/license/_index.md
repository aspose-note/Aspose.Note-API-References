---
title: Class License
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.License 班级. 提供许可组件的方法
type: docs
weight: 310
url: /zh/net/aspose.note/license/
---
## License class

提供许可组件的方法。

```csharp
public class License
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [License](license/)() | 默认构造函数。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | 许可组件。 |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | 许可组件。 |

### 例子

显示如何从文件加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

显示如何从流中加载 Aspose.Note 的许可证。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

显示如何从嵌入式文件资源加载 Aspose.Note 的许可证。

```csharp
// 实例化许可类
Aspose.Note.License license = new Aspose.Note.License();

// 仅传递程序集中嵌入的许可证文件的名称
license.SetLicense("Aspose.Note.lic");
```

### 也可以看看

* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


