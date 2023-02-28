---
title: TableColumn.LockedWidth
second_title: Aspose.Note .NET API संदर्भ के लिए
description: TableColumn संपत्त. एक मन प्रप्त करत है य सेट करत है ज इंगत करत है क तलक कलम में चड़ई बंद है और तलक समग्र क फट करने के लए स्वचलत रूप से आकर नहं बदलत है डफ़ल्ट रूप से कलम चड़ई लक नहं हत है
type: docs
weight: 20
url: /hi/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि तालिका कॉलम में चौड़ाई बंद है और तालिका सामग्री को फिट करने के लिए स्वचालित रूप से आकार नहीं बदलता है। डिफ़ॉल्ट रूप से, कॉलम चौड़ाई लॉक नहीं होती है।

```csharp
public bool LockedWidth { get; set; }
```

### उदाहरण

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

### यह सभी देखें

* class [TableColumn](../)
* नाम स्थान [Aspose.Note](../../tablecolumn/)
* सभा [Aspose.Note](../../../)


