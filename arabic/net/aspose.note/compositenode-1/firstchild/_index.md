---
title: "CompositeNode1.FirstChild"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية CompositeNode. تحصل على أول عقدة فرعية لهذا العقدة"
type: docs
weight: 10
url: /ar/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

يحصل على العقدة الفرعية الأولى لهذه العقدة.

```csharp
public T FirstChild { get; }
```

## أمثلة

يعرض كيفية التحقق مما إذا كانت الصفحة صفحة تعارض (أي أنها تحتوي على تغييرات لم يتمكن OneNote من دمجها تلقائيًا).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote.
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // بشكل افتراضي، يتم تخطي صفحات التعارض عند الحفظ.
    // إذا تم وضع علامة بأنها غير متعارضة، فسيتم حفظها كصفحة عادية في السجل.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### انظر أيضًا

* class [CompositeNode&lt;T&gt;](../)
* namespace [Aspose.Note](../../compositenode-1/)
* assembly [Aspose.Note](../../../)


