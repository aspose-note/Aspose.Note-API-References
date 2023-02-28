---
title: TableCell.BackgroundColor
second_title: Aspose.Note .NET API संदर्भ के लिए
description: TableCell संपत्त. पृष्ठभूम क रंग प्रप्त य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

पृष्ठभूमि का रंग प्राप्त या सेट करता है।

```csharp
public Color BackgroundColor { get; set; }
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

### यह सभी देखें

* class [TableCell](../)
* नाम स्थान [Aspose.Note](../../tablecell/)
* सभा [Aspose.Note](../../../)


