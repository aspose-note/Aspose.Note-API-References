---
title: "NumberList.FontSize"
second_title: "Aspose.Note for .NET API 参考"
description: "NumberList 属性。获取或设置字体大小。"
type: docs
weight: 40
url: /zh/net/aspose.note/numberlist/fontsize/
---
## NumberList.FontSize property

获取或设置字体大小。

```csharp
public int FontSize { get; set; }
```

## 示例

展示如何检索列表格式的信息。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// 检索大纲元素的节点集合
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 遍历每个节点
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 检索字体名称
        Console.WriteLine("Font Name: " + list.Font);

        // 检索字体长度
        Console.WriteLine("Font Length: " + list.Font.Length);

        // 检索字体大小
        Console.WriteLine("Font Size: " + list.FontSize);

        // 检索字体颜色
        Console.WriteLine("Font Color: " + list.FontColor);

        // 检索格式
        Console.WriteLine("Font format: " + list.Format);

        // 检查粗体
        Console.WriteLine("Is bold: " + list.IsBold);

        // 检查斜体
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### 另请参阅

* class [NumberList](../)
* namespace [Aspose.Note](../../numberlist/)
* assembly [Aspose.Note](../../../)


