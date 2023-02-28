---
title: Notebook.LoadChildDocument
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Notebook तरक. चइल्ड दस्तवेज़ नड जड़त है. फ़इल से मजूद OneNote दस्तवेज़ खलत है.
type: docs
weight: 120
url: /hi/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

चाइल्ड दस्तावेज़ नोड जोड़ता है. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है.

```csharp
public void LoadChildDocument(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |

### उदाहरण

दिखाता है कि स्ट्रीम से नोटबुक कैसे लोड करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### यह सभी देखें

* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

चाइल्ड दस्तावेज़ नोड जोड़ता है. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है. अतिरिक्त लोड विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |
| loadOptions | LoadOptions | लोड विकल्प। |

### यह सभी देखें

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

चाइल्ड दस्तावेज़ नोड जोड़ता है. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है.

```csharp
public void LoadChildDocument(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |

### उदाहरण

दिखाता है कि स्ट्रीम से नोटबुक कैसे लोड करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### यह सभी देखें

* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

चाइल्ड दस्तावेज़ नोड जोड़ता है. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है. अतिरिक्त लोड विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| loadOptions | LoadOptions | लोड विकल्प। |

### यह सभी देखें

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)


