---
title: Enum FileFormat
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.FileFormat एनुम. OneNote फ़इल स्वरूप क प्रतनधत्व करत है
type: docs
weight: 90
url: /hi/net/aspose.note/fileformat/
---
## FileFormat enumeration

OneNote फ़ाइल स्वरूप का प्रतिनिधित्व करता है।

```csharp
public enum FileFormat
```

### मान

| नाम | कीमत | विवरण |
| --- | --- | --- |
| Unknown | `0` | अज्ञात फ़ाइल स्वरूप. |
| OneNote2007 | `1` | वननोट 2010. |
| OneNote2010 | `2` | वननोट 2010. |
| OneNoteOnline | `3` | वननोट ऑनलाइन। |

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


