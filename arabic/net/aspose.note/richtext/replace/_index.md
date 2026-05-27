---
title: "RichText.Replace"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة RichText. تستبدل جميع تكرارات حرف يونيكود محدد في هذه النسخة بحرف يونيكود آخر محدد"
type: docs
weight: 230
url: /ar/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

يستبدل جميع تكرارات حرف يونيكود محدد في هذه الحالة بحرف يونيكود آخر محدد.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oldChar | Char | الحرف القديم. |
| newChar | Char | الحرف الجديد. |

### قيمة الإرجاع

ال[`RichText`](../).

### انظر أيضًا

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

يستبدل جميع تكرارات سلسلة محددة في الحالة الحالية بسلسلة أخرى محددة.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | String | القيمة القديمة. |
| newValue | String | القيمة الجديدة. |

### قيمة الإرجاع

ال[`RichText`](../).

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

## أمثلة

يوضح كيفية المرور عبر نص الصفحة وإجراء استبدال.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// احصل على جميع عقد RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // استبدال نص الشكل
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// احفظ بأي تنسيق ملف مدعوم
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يظهر كيفية إنشاء مستند جديد عن طريق استبدال قطع النص الخاصة في القالب.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// حمّل مستند القالب في Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// لنستبدل جميع كلمات القالب
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### انظر أيضًا

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

يستبدل جميع تكرارات سلسلة محددة في الحالة الحالية بسلسلة أخرى محددة بنمط محدد.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | String | القيمة القديمة. |
| newValue | String | القيمة الجديدة. |
| style | TextStyle | نمط القيمة الجديدة. |

### قيمة الإرجاع

ال[`RichText`](../).

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### انظر أيضًا

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


