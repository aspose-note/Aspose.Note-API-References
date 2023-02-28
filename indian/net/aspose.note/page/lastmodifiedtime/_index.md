---
title: Page.LastModifiedTime
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Page संपत्त. अंतम संशधत समय प्रप्त य सेट करत है
type: docs
weight: 60
url: /hi/net/aspose.note/page/lastmodifiedtime/
---
## Page.LastModifiedTime property

अंतिम संशोधित समय प्राप्त या सेट करता है।

```csharp
public DateTime LastModifiedTime { get; set; }
```

### उदाहरण

दिखाता है कि किसी पृष्ठ के बारे में मेटा जानकारी कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

दिखाता है कि पृष्ठ का इतिहास कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// पहला पेज प्राप्त करें
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### यह सभी देखें

* class [Page](../)
* नाम स्थान [Aspose.Note](../../page/)
* सभा [Aspose.Note](../../../)


