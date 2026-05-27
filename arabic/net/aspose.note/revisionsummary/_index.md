---
title: "فئة RevisionSummary"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "فئة Aspose.Note.RevisionSummary. تمثّل ملخصًا لتعديل العقد"
type: docs
weight: 600
url: /ar/net/aspose.note/revisionsummary/
---
## RevisionSummary class

يمثل ملخصًا لمراجعة العقدة.

```csharp
public class RevisionSummary
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | يحصل أو يعيّن المؤلف الأخير. |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |

## أمثلة

يعرض كيفية تعديل معلومات التعريف للصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// قراءة ملخص مراجعة المحتوى لهذه الصفحة.
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// تحديث ملخص مراجعة الصفحة لهذه الصفحة.
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


