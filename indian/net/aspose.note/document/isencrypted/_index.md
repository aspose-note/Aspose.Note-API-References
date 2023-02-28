---
title: Document.IsEncrypted
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. जंचत है क स्ट्रम से कई दस्तवेज़ एन्क्रप्ट कय गय है य नहं इसे जंचने के लए हमें इस दस्तवेज़ क पूर तरह लड करने क आवश्यकत है त इस वध से प्रदर्शन जुर्मन ह सकत है
type: docs
weight: 150
url: /hi/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

जांचता है कि स्ट्रीम से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है।

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| options | LoadOptions | लोड विकल्प। |
| document | Document& | लोड किया गया दस्तावेज़. |

### प्रतिलाभ की मात्रा

सही रिटर्न देता है यदि दस्तावेज़ एन्क्रिप्ट किया गया है अन्यथा गलत है।

### उदाहरण

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### यह सभी देखें

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

जांचता है कि स्ट्रीम से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है।

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| password | String | दस्तावेज़ को डिक्रिप्ट करने के लिए पासवर्ड. |
| document | Document& | लोड किया गया दस्तावेज़. |

### प्रतिलाभ की मात्रा

सही रिटर्न देता है यदि दस्तावेज़ एन्क्रिप्ट किया गया है अन्यथा गलत है।

### उदाहरण

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

जांचता है कि स्ट्रीम से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है।

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | स्ट्रीम. |
| document | Document& | लोड किया गया दस्तावेज़. |

### प्रतिलाभ की मात्रा

सही रिटर्न देता है यदि दस्तावेज़ एन्क्रिप्ट किया गया है अन्यथा गलत है।

### उदाहरण

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

जांचता है कि फ़ाइल से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है।

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |
| options | LoadOptions | लोड विकल्प। |
| document | Document& | लोड किया गया दस्तावेज़. |

### प्रतिलाभ की मात्रा

सही रिटर्न देता है यदि दस्तावेज़ एन्क्रिप्ट किया गया है अन्यथा गलत है।

### उदाहरण

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### यह सभी देखें

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

जांचता है कि फ़ाइल से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है।

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |
| document | Document& | लोड किया गया दस्तावेज़. |

### प्रतिलाभ की मात्रा

सही रिटर्न देता है यदि दस्तावेज़ एन्क्रिप्ट किया गया है अन्यथा गलत है।

### उदाहरण

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

जांचता है कि फ़ाइल से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है।

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल पथ. |
| password | String | दस्तावेज़ को डिक्रिप्ट करने के लिए पासवर्ड. |
| document | Document& | लोड किया गया दस्तावेज़. |

### प्रतिलाभ की मात्रा

सही रिटर्न देता है यदि दस्तावेज़ एन्क्रिप्ट किया गया है अन्यथा गलत है।

### उदाहरण

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


