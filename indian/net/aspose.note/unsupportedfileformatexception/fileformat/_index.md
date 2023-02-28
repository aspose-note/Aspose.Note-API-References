---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note .NET API संदर्भ के लिए
description: UnsupportedFileFormatException संपत्त. पत चलने पर परत डेट क फ़इल प्ररूप प्रप्त करत है
type: docs
weight: 10
url: /hi/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

पता चलने पर पारित डेटा का फ़ाइल प्रारूप प्राप्त करता है।

```csharp
public FileFormat FileFormat { get; }
```

### उदाहरण

दिखाता है कि कैसे जांचें कि दस्तावेज़ लोड विफल हो गया है क्योंकि OneNote 2007 प्रारूप समर्थित नहीं है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### यह सभी देखें

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* नाम स्थान [Aspose.Note](../../unsupportedfileformatexception/)
* सभा [Aspose.Note](../../../)


