---
title: "CompositeNode1.GetChildNodes"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة CompositeNode. احصل على جميع العقد الفرعية حسب نوع العقدة"
type: docs
weight: 70
url: /ar/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

احصل على جميع عقد الطفل حسب نوع العقدة.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| معامل | الوصف |
| --- | --- |
| T1 | نوع العناصر في القائمة المعادة. |

### قيمة الإرجاع

قائمة من العقد الفرعية.

## أمثلة

يظهر كيفية الحصول على صورة من مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // حفظ بايتات الصورة إلى ملف
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

يظهر كيفية الحصول على معلومات ميتا للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

### انظر أيضًا

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* namespace [Aspose.Note](../../compositenode-1/)
* assembly [Aspose.Note](../../../)


