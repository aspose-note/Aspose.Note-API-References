---
title: CompositeNode1.FirstChild
second_title: Aspose.Note لمرجع NET API
description: CompositeNode ملكية. الحصول على العقدة الفرعية الأولى لهذه العقدة .
type: docs
weight: 10
url: /ar/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

الحصول على العقدة الفرعية الأولى لهذه العقدة .

```csharp
public T FirstChild { get; }
```

### أمثلة

يوضح كيفية التحقق مما إذا كانت الصفحة عبارة عن صفحة تعارض (أي أنها تحتوي على تغييرات يتعذر على OneNote دمجها تلقائيًا).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote
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

    // بشكل افتراضي يتم تخطي صفحات التعارض فقط عند الحفظ.
    // إذا قمت بتمييزه على أنه غير متعارض ، فسيتم حفظه كالمعتاد في السجل.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### أنظر أيضا

* class [CompositeNode&lt;T&gt;](../)
* مساحة الاسم [Aspose.Note](../../compositenode-1/)
* المجسم [Aspose.Note](../../../)


