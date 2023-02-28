---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.UnsupportedFileFormatException कक्ष. दस्तवेज़ लड के दरन फेंक जत है जब फ़इल स्वरूप पहचन नहं जत है य Aspose.Note. द्वर समर्थत नहं है
type: docs
weight: 990
url: /hi/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

दस्तावेज़ लोड के दौरान फेंका जाता है, जब फ़ाइल स्वरूप पहचाना नहीं जाता है या Aspose.Note. द्वारा समर्थित नहीं है

```csharp
public class UnsupportedFileFormatException : Exception
```

## गुण

| नाम | विवरण |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | पता चलने पर पारित डेटा का फ़ाइल प्रारूप प्राप्त करता है। |

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

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


