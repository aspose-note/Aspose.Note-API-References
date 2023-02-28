---
title: Notebook.Save
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Notebook तरक. OneNote दस्तवेज़ क फ़इल में सहेजत है.
type: docs
weight: 150
url: /hi/net/aspose.note/notebook/save/
---
## Save(string) {#save_3}

OneNote दस्तावेज़ को फ़ाइल में सहेजता है.

```csharp
public void Save(string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | फ़ाइल का पूरा नाम। यदि निर्दिष्ट पूर्ण नाम वाली फ़ाइल पहले से मौजूद है, तो मौजूदा फ़ाइल अधिलेखित हो जाती है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## Save(Stream) {#save}

OneNote दस्तावेज़ को स्ट्रीम में सहेजता है.

```csharp
public void Save(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

OneNote दस्तावेज़ को निर्दिष्ट स्वरूप में फ़ाइल में सहेजता है.

```csharp
public void Save(string fileName, SaveFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | फ़ाइल का पूरा नाम। यदि निर्दिष्ट पूर्ण नाम वाली फ़ाइल पहले से मौजूद है, तो मौजूदा फ़ाइल अधिलेखित हो जाती है. |
| format | SaveFormat | वह प्रारूप जिसमें दस्तावेज़ को सहेजना है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

निर्दिष्ट प्रारूप में एक स्ट्रीम में OneNote दस्तावेज़ सहेजता है।

```csharp
public void Save(Stream stream, SaveFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| format | SaveFormat | वह प्रारूप जिसमें दस्तावेज़ को सहेजना है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## Save(string, NotebookSaveOptions) {#save_5}

निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को फ़ाइल में सहेजता है.

```csharp
public void Save(string fileName, NotebookSaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | फ़ाइल का पूरा नाम। यदि निर्दिष्ट पूर्ण नाम वाली फ़ाइल पहले से मौजूद है, तो मौजूदा फ़ाइल अधिलेखित हो जाती है. |
| options | NotebookSaveOptions | दस्तावेज़ को फ़ाइल में सहेजे जाने के विकल्पों को निर्दिष्ट करता है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)

---

## Save(Stream, NotebookSaveOptions) {#save_2}

निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को स्ट्रीम में सहेजता है.

```csharp
public void Save(Stream stream, NotebookSaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| options | NotebookSaveOptions | दस्तावेज़ को सहेजे जाने के विकल्पों को निर्दिष्ट करता है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)


