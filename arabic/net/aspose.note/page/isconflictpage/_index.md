---
title: "Page.IsConflictPage"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Page. يحصل أو يحدد قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض"
type: docs
weight: 50
url: /ar/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

يحصل أو يضبط قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض.

```csharp
public bool IsConflictPage { get; set; }
```

## ملاحظات

تظهر صفحة التعارض عندما يحاول مستخدمان تحديث نفس المحتوى. في هذه الحالة تُكتب تغييرات المستخدم الأول كالمعتاد. لكن لا يمكن دمج تغييرات المستخدم الآخر. لذلك يتم إنشاء نسخة من الصفحة وتحديدها كتعارض.

في هذا الإصدار يتم حل التعارضات لصالح تغييرات المستخدم الأول. لذا إذا كان المستند يحتوي على صفحات تعارض فسيتم عرضها في السجل لكنها ستُتخطى عند الحفظ. يمكن إعادة ضبط هذه العلامة لحفظ هذه الصفحات في السجل كصفحات عادية.

يمكن العثور على مثال تفصيلي للتعامل مع صفحة التعارض في الوثائق عبر الإنترنت.

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

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


