---
title: Document.Document
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document नर्मत. क एक नय उदहरण प्ररंभ करत हैDocument class. एक रक्त OneNote दस्तवेज़ बनत है.
type: docs
weight: 10
url: /hi/net/aspose.note/document/document/
---
## Document() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`Document`](../) class. एक रिक्त OneNote दस्तावेज़ बनाता है.

```csharp
public Document()
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

का एक नया उदाहरण प्रारंभ करता है[`Document`](../) class. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है.

```csharp
public Document(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | दस्तावेज़ प्रारूप पहचाना नहीं गया है या समर्थित नहीं है। |
| [FileCorruptedException](../../filecorruptedexception/) | दस्तावेज़ दूषित प्रतीत होता है और लोड नहीं किया जा सकता। |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | दस्तावेज़ एन्क्रिप्ट किया गया है और खोलने के लिए पासवर्ड की आवश्यकता है, लेकिन आपने गलत पासवर्ड प्रदान किया है। |
| InvalidOperationException | दस्तावेज़ में कोई समस्या है और इसकी रिपोर्ट Aspose.Note डेवलपर्स को की जानी चाहिए। |
| IOException | एक इनपुट/आउटपुट अपवाद है। |

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

का एक नया उदाहरण प्रारंभ करता है[`Document`](../)class. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है। एन्क्रिप्शन पासवर्ड जैसे अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |
| loadOptions | LoadOptions | दस्तावेज़ लोड करने के लिए उपयोग किए जाने वाले विकल्प। रिक्त हो सकता है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | दस्तावेज़ प्रारूप पहचाना नहीं गया है या समर्थित नहीं है। |
| [FileCorruptedException](../../filecorruptedexception/) | दस्तावेज़ दूषित प्रतीत होता है और लोड नहीं किया जा सकता। |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | दस्तावेज़ एन्क्रिप्ट किया गया है और खोलने के लिए पासवर्ड की आवश्यकता है, लेकिन आपने गलत पासवर्ड प्रदान किया है। |
| InvalidOperationException | दस्तावेज़ में कोई समस्या है और इसकी रिपोर्ट Aspose.Note डेवलपर्स को की जानी चाहिए। |
| IOException | एक इनपुट/आउटपुट अपवाद है। |

### यह सभी देखें

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Document`](../) class. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है.

```csharp
public Document(Stream inStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| inStream | Stream | स्ट्रीम. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | दस्तावेज़ प्रारूप पहचाना नहीं गया है या समर्थित नहीं है। |
| [FileCorruptedException](../../filecorruptedexception/) | दस्तावेज़ दूषित प्रतीत होता है और लोड नहीं किया जा सकता। |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | दस्तावेज़ एन्क्रिप्ट किया गया है और खोलने के लिए पासवर्ड की आवश्यकता है, लेकिन आपने गलत पासवर्ड प्रदान किया है। |
| InvalidOperationException | दस्तावेज़ में कोई समस्या है और इसकी रिपोर्ट Aspose.Note डेवलपर्स को की जानी चाहिए। |
| IOException | एक इनपुट/आउटपुट अपवाद है। |
| ArgumentException | धारा पढ़ने का समर्थन नहीं करती, अशक्त है, या पहले से ही बंद है। |

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`Document`](../) class. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है। एन्क्रिप्शन पासवर्ड जैसे अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| inStream | Stream | स्ट्रीम. |
| loadOptions | LoadOptions | दस्तावेज़ लोड करने के लिए उपयोग किए जाने वाले विकल्प। रिक्त हो सकता है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | दस्तावेज़ प्रारूप पहचाना नहीं गया है या समर्थित नहीं है। |
| [FileCorruptedException](../../filecorruptedexception/) | दस्तावेज़ दूषित प्रतीत होता है और लोड नहीं किया जा सकता। |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | दस्तावेज़ एन्क्रिप्ट किया गया है और खोलने के लिए पासवर्ड की आवश्यकता है, लेकिन आपने गलत पासवर्ड प्रदान किया है। |
| InvalidOperationException | दस्तावेज़ में कोई समस्या है और इसकी रिपोर्ट Aspose.Note डेवलपर्स को की जानी चाहिए। |
| IOException | एक इनपुट/आउटपुट अपवाद है। |
| ArgumentException | धारा पढ़ने का समर्थन नहीं करती, अशक्त है, या पहले से ही बंद है। |

### यह सभी देखें

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


