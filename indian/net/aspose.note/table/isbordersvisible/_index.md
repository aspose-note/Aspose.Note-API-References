---
title: Table.IsBordersVisible
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Table संपत्त. एक मन प्रप्त करत है य सेट करत है ज इंगत करत है क तलक सम दृश्यमन है य नहं
type: docs
weight: 30
url: /hi/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि तालिका सीमा दृश्यमान है या नहीं।

```csharp
public bool IsBordersVisible { get; set; }
```

### उदाहरण

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

* class [Table](../)
* नाम स्थान [Aspose.Note](../../table/)
* सभा [Aspose.Note](../../../)


