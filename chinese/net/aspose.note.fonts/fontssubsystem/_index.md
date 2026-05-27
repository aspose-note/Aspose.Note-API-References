---
title: "类 FontsSubsystem"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Fonts.FontsSubsystem 类。实现 Aspose.Note.Fonts.IFontsSubsystem 接口的基类。提供默认字体和字体替换的功能。在派生类中重写 Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily 受保护成员函数，以实现获取 FontFamily 对象的逻辑。"
type: docs
weight: 110
url: /zh/net/aspose.note.fonts/fontssubsystem/
---
## FontsSubsystem class

实现 Aspose.Note.Fonts.IFontsSubsystem 接口的基类。提供默认字体及字体替换的功能。在派生类中重写 Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily 受保护成员函数，以实现检索 FontFamily 对象的逻辑。

```csharp
public abstract class FontsSubsystem : IFontsSubsystem
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | 获取或设置默认字体。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont)(Stream) | 添加字体。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_2)(string) | 添加字体。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_1)(Stream, string) | 添加字体。 |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | 添加字体替换。 |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | 获取字体系列。 |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | 从指定文件夹加载所有 TrueType 字体到内部集合。 |

### 另请参阅

* interface [IFontsSubsystem](../ifontssubsystem/)
* namespace [Aspose.Note.Fonts](../../aspose.note.fonts/)
* assembly [Aspose.Note](../../)


