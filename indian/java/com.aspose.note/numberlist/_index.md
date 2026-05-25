---
title: "NumberList"
second_title: "Aspose.Note for Java API Reference"
description: "Represents the numbered or bulleted list."
type: docs
weight: 64
url: /hi/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Represents the numbered or bulleted list.
## Constructors

| Constructor | Description |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | `NumberList` क्लास की नई इंस्टेंस को प्रारंभ करता है। |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | `NumberList` क्लास की नई इंस्टेंस को प्रारंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | निर्धारित करता है कि निर्दिष्ट ऑब्जेक्ट वर्तमान ऑब्जेक्ट के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | निर्धारित करता है कि निर्दिष्ट ऑब्जेक्ट वर्तमान ऑब्जेक्ट के बराबर है या नहीं। |
| [getFont()](#getFont--) | फ़ॉन्ट का नाम प्राप्त करता है या सेट करता है। |
| [getFontColor()](#getFontColor--) | फ़ॉन्ट रंग प्राप्त करता है या सेट करता है. |
| [getFontSize()](#getFontSize--) | फ़ॉन्ट आकार प्राप्त करता है या सेट करता है। |
| [getFormat()](#getFormat--) | लाइन हेडर का फ़ॉर्मेट प्राप्त करता है या सेट करता है। |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getNumberFormat()](#getNumberFormat--) | स्वचालित रूप से क्रमांकित वस्तुओं के समूह के लिए उपयोग किए जाने वाले संख्या फ़ॉर्मेट को प्राप्त करता है या सेट करता है। |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | क्रमांकित सूची हेडर प्राप्त करता है। |
| [getRestart()](#getRestart--) | सूची आइटम के स्वचालित संख्या मान को ओवरराइड करने वाला संख्यात्मक मान प्राप्त करता है या सेट करता है। |
| [hashCode()](#hashCode--) | प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है. |
| [isBold()](#isBold--) | पाठ शैली बोल्ड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [isItalic()](#isItalic--) | पाठ शैली इटैलिक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [setBold(boolean value)](#setBold-boolean-) | पाठ शैली बोल्ड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [setFont(String value)](#setFont-java.lang.String-) | फ़ॉन्ट का नाम प्राप्त करता है या सेट करता है। |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | फ़ॉन्ट रंग प्राप्त करता है या सेट करता है. |
| [setFontSize(int value)](#setFontSize-int-) | फ़ॉन्ट आकार प्राप्त करता है या सेट करता है। |
| [setFormat(String value)](#setFormat-java.lang.String-) | लाइन हेडर का फ़ॉर्मेट प्राप्त करता है या सेट करता है। |
| [setItalic(boolean value)](#setItalic-boolean-) | पाठ शैली इटैलिक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | स्वचालित रूप से क्रमांकित वस्तुओं के समूह के लिए उपयोग किए जाने वाले संख्या फ़ॉर्मेट को प्राप्त करता है या सेट करता है। |
| [setRestart(int value)](#setRestart-int-) | सूची आइटम के स्वचालित संख्या मान को ओवरराइड करने वाला संख्यात्मक मान प्राप्त करता है या सेट करता है। |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


`NumberList` क्लास की नई इंस्टेंस को प्रारंभ करता है। यह इंस्टेंस बुलेटेड सूची का प्रतिनिधित्व करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | एक प्रतीक जो बुलेट का प्रतिनिधित्व करता है। |
| font | java.lang.String | बुलेट के लिए फ़ॉन्ट। |
| fontSize | int | बुलेट के लिए फ़ॉन्ट आकार। |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


`NumberList` क्लास की नई इंस्टेंस को प्रारंभ करता है। यह इंस्टेंस क्रमांकित सूची का प्रतिनिधित्व करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | java.lang.String | क्रमांकित हेडर का फ़ॉर्मेट। |
| numberFormat | byte | हेडर में संख्या का प्रारूप। |
| font | java.lang.String | क्रमांकित हेडर के लिए फ़ॉन्ट। |
| fontSize | int | क्रमांकित हेडर के लिए फ़ॉन्ट आकार। |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


निर्धारित करता है कि निर्दिष्ट ऑब्जेक्ट वर्तमान ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | The object. |

**Returns:**
boolean - The `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


निर्धारित करता है कि निर्दिष्ट ऑब्जेक्ट वर्तमान ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object. |

**Returns:**
boolean - The `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


फ़ॉन्ट का नाम प्राप्त करता है या सेट करता है।

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


फ़ॉन्ट रंग प्राप्त करता है या सेट करता है.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


फ़ॉन्ट आकार प्राप्त करता है या सेट करता है।

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


लाइन हेडर का प्रारूप प्राप्त करता है या सेट करता है। बुलेटेड सूचियों के लिए बुलेट प्रतीक दर्शाता है।

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


स्वचालित रूप से क्रमांकित वस्तुओं के समूह के लिए उपयोग किए जाने वाले संख्या प्रारूप को प्राप्त करता है या सेट करता है। बुलेटेड सूचियों के लिए इसे null होना चाहिए।

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


क्रमांकित सूची हेडर प्राप्त करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sequenceNumber | int | क्रमांकित सूची में क्रम संख्या। |

**Returns:**
java.lang.String - निर्दिष्ट क्रम संख्या का स्ट्रिंग प्रतिनिधित्व।
### getRestart() {#getRestart--}
```
public int getRestart()
```


सूची आइटम के स्वचालित संख्या मान को ओवरराइड करने वाला संख्यात्मक मान प्राप्त करता है या सेट करता है।

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है.

**Returns:**
int - The `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


पाठ शैली बोल्ड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


पाठ शैली इटैलिक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


पाठ शैली बोल्ड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


फ़ॉन्ट का नाम प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


फ़ॉन्ट रंग प्राप्त करता है या सेट करता है.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


फ़ॉन्ट आकार प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


लाइन हेडर का प्रारूप प्राप्त करता है या सेट करता है। बुलेटेड सूचियों के लिए बुलेट प्रतीक दर्शाता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


पाठ शैली इटैलिक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


स्वचालित रूप से क्रमांकित वस्तुओं के समूह के लिए उपयोग किए जाने वाले संख्या प्रारूप को प्राप्त करता है या सेट करता है। बुलेटेड सूचियों के लिए इसे null होना चाहिए।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


सूची आइटम के स्वचालित संख्या मान को ओवरराइड करने वाला संख्यात्मक मान प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

