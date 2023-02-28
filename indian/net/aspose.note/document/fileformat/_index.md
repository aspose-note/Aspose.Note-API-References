---
title: Document.FileFormat
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document संपत्त. फ़इल स्वरूप प्रप्त करत है OneNote 2010 OneNote ऑनलइन
type: docs
weight: 60
url: /hi/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

फ़ाइल स्वरूप प्राप्त करता है (OneNote 2010, OneNote ऑनलाइन)।

```csharp
public FileFormat FileFormat { get; }
```

### उदाहरण

दस्तावेज़ का फ़ाइल स्वरूप प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // प्रक्रिया OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // प्रक्रिया OneNote ऑनलाइन
        break;
}
```

### यह सभी देखें

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


