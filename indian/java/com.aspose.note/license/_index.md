---
title: "License"
second_title: "Aspose.Note for Java API Reference"
description: "Provides methods to license the component."
type: docs
weight: 44
url: /hi/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Provides methods to license the component.
## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | इस क्लास का नया उदाहरण आरंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | वर्तमान थ्रेड के लिए लाइसेंस कॉन्टेक्स्ट को रीसेट करता है। |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | घटक को लाइसेंस देता है। |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | घटक को लाइसेंस देता है। |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | घटक को लाइसेंस देता है। |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | वर्तमान थ्रेड के लिए लाइसेंस कॉन्टेक्स्ट सेट करता है। |
### License() {#License--}
```
public License()
```


इस क्लास का नया उदाहरण आरंभ करता है।

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


वर्तमान थ्रेड के लिए लाइसेंस कॉन्टेक्स्ट को रीसेट करता है।

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


घटक को लाइसेंस देता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseFile | java.io.File | लाइसेंस फ़ाइल`System.IO.FileInfo`। |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


घटक को लाइसेंस देता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | एक स्ट्रीम जिसमें लाइसेंस शामिल है। |

--------------------

`

इस विधि का उपयोग करके स्ट्रीम से लाइसेंस लोड करें।

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


घटक को लाइसेंस देता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | licenseName | java.lang.String | पूरा या छोटा फ़ाइल नाम` या एम्बेडेड रिसोर्स का नाम`. मूल्यांकन मोड में स्विच करने के लिए खाली स्ट्रिंग का उपयोग करें। |

--------------------

`

लाइसेंस को निम्नलिखित स्थानों में खोजने का प्रयास करता है:

` `

1. स्पष्ट पथ।

` `

2. वह फ़ोल्डर जिसमें Aspose घटक असेंबली शामिल है।

3. वह फ़ोल्डर जिसमें क्लाइंट की कॉलिंग असेंबली शामिल है।

4. वह फ़ोल्डर जिसमें एंट्री (स्टार्टअप) असेंबली शामिल है।

5. क्लाइंट की कॉलिंग असेंबली में एक एम्बेडेड रिसोर्स।

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. स्पष्ट पथ।

2. क्लाइंट की कॉलिंग असेंबली में एक एम्बेडेड रिसोर्स।

` `

2. वह फ़ोल्डर जिसमें Aspose घटक JAR फ़ाइल शामिल है।

3. वह फ़ोल्डर जिसमें क्लाइंट की कॉलिंग JAR फ़ाइल शामिल है।

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


वर्तमान थ्रेड के लिए लाइसेंस कॉन्टेक्स्ट सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | एक स्ट्रीम जिसमें लाइसेंस शामिल है। |

