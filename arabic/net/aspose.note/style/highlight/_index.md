---
title: Style.Highlight
second_title: Aspose.Note لمرجع NET API
description: Style ملكية. الحصول على لون التمييز أو تعيينه.
type: docs
weight: 50
url: /ar/net/aspose.note/style/highlight/
---
## Style.Highlight property

الحصول على لون التمييز أو تعيينه.

```csharp
public Color Highlight { get; set; }
```

### أمثلة

يوضح كيفية تغيير نمط النص.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// احصل على عقدة RichText معينة
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // تعيين لون الخط
    run.Style.FontColor = Color.Yellow;

    // تعيين لون التظليل
    run.Style.Highlight = Color.Blue;

    // تعيين حجم الخط
    run.Style.FontSize = 20;
}
```

يوضح كيفية إنشاء جدول يحتوي على نص بأنماط مختلفة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// نص الملخص قبل الجدول
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// دعنا نضيف مجموعة من الأعمدة وصف الرأس
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// دعونا 5 صفوف فارغة. الصفوف لها لون خلفية متبادل
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// دعنا نضيف بعض النماذج للمحتوى في عمود "جهات الاتصال"
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

### أنظر أيضا

* class [Style](../)
* مساحة الاسم [Aspose.Note](../../style/)
* المجسم [Aspose.Note](../../../)


