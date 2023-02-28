---
title: NumberList.Format
second_title: Aspose.Note for .NET API 参考
description: NumberList 财产. 获取或设置行标题的格式对于项目符号列表表示项目符号
type: docs
weight: 50
url: /zh/net/aspose.note/numberlist/format/
---
## NumberList.Format property

获取或设置行标题的格式。对于项目符号列表表示项目符号。

```csharp
public string Format { get; set; }
```

### 例子

显示如何检索有关列表格式的信息。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// 检索轮廓元素的集合节点
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

//遍历每个节点
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 检索字体名称
        Console.WriteLine("Font Name: " + list.Font);

        // 获取字体长度
        Console.WriteLine("Font Length: " + list.Font.Length);

        // 获取字体大小
        Console.WriteLine("Font Size: " + list.FontSize);

        // 获取字体颜色
        Console.WriteLine("Font Color: " + list.FontColor);

        // 检索格式
        Console.WriteLine("Font format: " + list.Format);

        // 勾选粗体
        Console.WriteLine("Is bold: " + list.IsBold);

        // 检查斜体
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### 也可以看看

* class [NumberList](../)
* 命名空间 [Aspose.Note](../../numberlist/)
* 部件 [Aspose.Note](../../../)


