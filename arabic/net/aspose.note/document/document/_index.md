---
title: "Document.Document"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "منشئ Document. يهيئ نسخة جديدة من فئة Document. ينشئ مستند OneNote فارغ"
type: docs
weight: 10
url: /ar/net/aspose.note/document/document/
---
## Document() {#constructor}

يهيئ نسخة جديدة من الفئة [`Document`](../). ينشئ مستند OneNote فارغ.

```csharp
public Document()
```

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

يهيئ نسخة جديدة من الفئة [`Document`](../). يفتح مستند OneNote موجود من ملف.

```csharp
public Document(string filePath)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معترف به أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور للفتح، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | هناك مشكلة في المستند ويجب الإبلاغ عنها لمطوري Aspose.Note. |
| IOException | هناك استثناء في الإدخال/الإخراج. |

## أمثلة

يوضح كيفية تحويل مستند OneNote إلى HTML متوافق مع Notion.

```csharp
var dataDir = RunExamples.GetDataDir_Import();
var documentPath = Path.Combine(dataDir, "Sample.one");

// تهيئة مستند OneNote.
var document = new Document(documentPath);

// إعداد عميل Notion
var authToken = "your-notion-auth-token";
var parentPageId = "your-notion-parent-page-id";

var client = NotionClientFactory.Create(new ClientOptions
{
    AuthToken = authToken
});

// استرجاع صفحة Notion
var page = await client.Pages.RetrieveAsync(parentPageId);

// التكرار على صفحات OneNote وإضافتها إلى Notion
foreach (var oneNotePage in document)
{
    var oneNoteAllRichText = oneNotePage.GetChildNodes<RichText>();

    var pagesCreateParametersBuilder = PagesCreateParametersBuilder
        .Create(new ParentPageInput { PageId = page.Id })
        .AddProperty("title",
        new TitlePropertyValue
        {
            Title = new List<RichTextBase>
            {
            new RichTextTextInput { Text = new Notion.Client.Text { Content = oneNotePage.Title.TitleText.Text } }
            }
        });

    foreach (var richText in oneNoteAllRichText)
    {
        // تجاوز النصوص الخاصة بالعنوان أو التاريخ أو الوقت
        if (richText.IsTitleDate || richText.IsTitleText || richText.IsTitleTime)
        {
            continue;
        }

        pagesCreateParametersBuilder.AddPageContent(new ParagraphBlock
        {
            Paragraph = new ParagraphBlock.Info
            {
                RichText = new List<RichTextBase> {
                new RichTextText
                {
                    Text = new Notion.Client.Text { Content = richText.Text }
                }
            }
            }
        });
    }

    // إنشاء صفحة في Notion
    var pagesCreateParameters = pagesCreateParametersBuilder.Build();
    await client.Pages.CreateAsync(pagesCreateParameters);
}

Console.WriteLine("\nOneNote document converted to Notion-compatible format successfully.");
```

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

يهيئ نسخة جديدة من الفئة [`Document`](../). يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| loadOptions | LoadOptions | الخيارات المستخدمة لتحميل مستند. يمكن أن تكون null. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معترف به أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور للفتح، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | هناك مشكلة في المستند ويجب الإبلاغ عنها لمطوري Aspose.Note. |
| IOException | هناك استثناء في الإدخال/الإخراج. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

يُنشئ مثيلاً جديدًا من الفئة [`Document`](../). يفتح مستند OneNote موجود من تدفق.

```csharp
public Document(Stream inStream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| inStream | Stream | التدفق. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معترف به أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور للفتح، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | هناك مشكلة في المستند ويجب الإبلاغ عنها لمطوري Aspose.Note. |
| IOException | هناك استثناء في الإدخال/الإخراج. |
| ArgumentException | التدفق لا يدعم القراءة، أو أنه فارغ، أو أنه مغلق بالفعل. |

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

يُنشئ مثيلاً جديدًا من الفئة [`Document`](../). يفتح مستند OneNote موجود من تدفق. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| inStream | Stream | التدفق. |
| loadOptions | LoadOptions | الخيارات المستخدمة لتحميل مستند. يمكن أن تكون null. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معترف به أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور للفتح، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | هناك مشكلة في المستند ويجب الإبلاغ عنها لمطوري Aspose.Note. |
| IOException | هناك استثناء في الإدخال/الإخراج. |
| ArgumentException | التدفق لا يدعم القراءة، أو أنه فارغ، أو أنه مغلق بالفعل. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


