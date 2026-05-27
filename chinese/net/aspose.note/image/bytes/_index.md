---
title: "Image.Bytes"
second_title: "Aspose.Note for .NET API 参考"
description: "Image 属性。获取图像数据存储"
type: docs
weight: 50
url: /zh/net/aspose.note/image/bytes/
---
## Image.Bytes property

获取图像数据存储。

```csharp
public byte[] Bytes { get; }
```

## 示例

展示如何从文档中获取图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有 Image 节点
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 将图像字节保存到文件
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### 另请参阅

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


