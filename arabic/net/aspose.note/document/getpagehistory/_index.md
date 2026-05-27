---
title: "Document.GetPageHistory"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Document. تحصل على PageHistory التي تحتوي على السجل الكامل لكل صفحة معروضة في المستند، الأقدم في الفهرس 0. يمكن الوصول إلى نسخة الصفحة الحالية كـ Current وتكون منفصلة عن مجموعة الإصدارات التاريخية."
type: docs
weight: 100
url: /ar/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

يحصل على [`PageHistory`](../../pagehistory/) التي تحتوي على السجل الكامل لكل صفحة معروضة في المستند (الأقدم في الفهرس 0). يمكن الوصول إلى نسخة الصفحة الحالية كـ [`Current`](../../pagehistory/current/) وتكون منفصلة عن مجموعة الإصدارات التاريخية.

```csharp
public PageHistory GetPageHistory(Page page)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| page | Page | الإصدار الحالي لصفحة. |

### قيمة الإرجاع

الـ [`PageHistory`](../../pagehistory/).

## أمثلة

يعرض كيفية استعادة النسخة السابقة لصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

يوضح كيفية تعديل تاريخ الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page();
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page());

    pageHistory.Insert(1, new Page());

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


