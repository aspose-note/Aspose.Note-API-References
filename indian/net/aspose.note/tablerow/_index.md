---
title: Class TableRow
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.TableRow कक्ष. तलक पंक्त क प्रतनधत्व करत है
type: docs
weight: 930
url: /hi/net/aspose.note/tablerow/
---
## TableRow class

तालिका पंक्ति का प्रतिनिधित्व करता है।

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TableRow](tablerow/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`TableRow` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablerow/lastmodifiedtime/) { get; set; } | अंतिम संशोधित समय प्राप्त या सेट करता है। |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Accept](../../aspose.note/tablerow/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableCell&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableCell[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### उदाहरण

दिखाता है कि प्रत्येक तालिका की पंक्ति से टेक्स्ट कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Sample1.one");

// टेबल नोड्स की सूची प्राप्त करें
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // तालिका पंक्तियों के माध्यम से पुनरावृति करें
    foreach (TableRow row in table)
    {
        // पाठ पुनर्प्राप्त करें
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
        Console.WriteLine(text);
    }
}
```

टेबल के सेल से टेक्स्ट प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Sample1.one");

// टेबल नोड्स की सूची प्राप्त करें
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // तालिका पंक्तियों के माध्यम से पुनरावृति करें
    foreach (TableRow row in table)
    {
        // टेबलसेल नोड्स की सूची प्राप्त करें
        // तालिका कक्षों के माध्यम से पुनरावृति करें
        foreach (TableCell cell in row)
        {
            // पाठ पुनर्प्राप्त करें
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
            Console.WriteLine(text);
        }
    }
}
```

सेल के लिए बैकग्राउंड कलर सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// टेबलसेल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट कंटेंट सेट करें
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableRow row = new TableRow(doc);
row.AppendChildLast(cell11);

Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement(doc);
oe.AppendChildLast(table);

Outline o = new Outline(doc);
o.AppendChildLast(oe);

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

टैग के साथ नई तालिका जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableRow row = new TableRow(doc);

// टेबलसेल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableCell cell = new TableCell(doc);

// सेल सामग्री डालें
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// पंक्ति नोड में सेल जोड़ें
row.AppendChildLast(cell);

// टेबल नोड को इनिशियलाइज़ करें
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// तालिका में पंक्ति नोड डालें
table.AppendChildLast(row);

// इस टेबल नोड में टैग जोड़ें
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// टेबल नोड जोड़ें
outlineElem.AppendChildLast(table);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

लॉक किए गए कॉलम के साथ टेबल बनाने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableRow row1 = new TableRow(doc);

// टेबलसेल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट कंटेंट सेट करें
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// TableRow क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableRow row2 = new TableRow(doc);

// टेबलसेल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट कंटेंट सेट करें
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// टेबल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// पंक्तियां जोड़ें
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// टेबल नोड जोड़ें
outlineElem.AppendChildLast(table);

// रूपरेखा तत्व नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

दिखाता है कि एक नई तालिका कैसे बनाई जाती है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tables();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// TableRow क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableRow row1 = new TableRow(doc);

// टेबलसेल क्लास ऑब्जेक्ट्स को इनिशियलाइज़ करें
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// टेबल सेल में आउटलाइन एलिमेंट्स जोड़ें
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// तालिका कक्ष पंक्तियों के लिए
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// TableRow क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
TableRow row2 = new TableRow(doc);

// टेबलसेल क्लास ऑब्जेक्ट्स को इनिशियलाइज़ करें
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// टेबल सेल में आउटलाइन एलिमेंट्स जोड़ें
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// तालिका कक्षों को पंक्तियों में जोड़ें
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// टेबल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और कॉलम की चौड़ाई सेट करें
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// तालिका पंक्तियों को तालिका में जोड़ें
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// आउटलाइन ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// एलिमेंट नोड को आउटलाइन करने के लिए टेबल जोड़ें
outlineElem.AppendChildLast(table);

// रूपरेखा तत्व को रूपरेखा में जोड़ें
outline.AppendChildLast(outlineElem);

// पेज नोड में रूपरेखा जोड़ें
page.AppendChildLast(outline);

// दस्तावेज़ नोड में पृष्ठ जोड़ें
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### यह सभी देखें

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableCell](../tablecell/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


