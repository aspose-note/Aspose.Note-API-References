---
title: RevisionSummary.LastModifiedTime
second_title: Aspose.Note لمرجع NET API
description: RevisionSummary ملكية. الحصول على أو تعيين وقت آخر تعديل.
type: docs
weight: 30
url: /ar/net/aspose.note/revisionsummary/lastmodifiedtime/
---
## RevisionSummary.LastModifiedTime property

الحصول على أو تعيين وقت آخر تعديل.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### أمثلة

يوضح كيفية تحرير المعلومات الوصفية للصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// قراءة ملخص مراجعة المحتوى لهذه الصفحة
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// تحديث ملخص مراجعة الصفحة لهذه الصفحة
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

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

* class [RevisionSummary](../)
* مساحة الاسم [Aspose.Note](../../revisionsummary/)
* المجسم [Aspose.Note](../../../)


