---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note for Java API Reference"
description: "Represents helper class with user-friednly interface to with AttributeSet."
type: docs
weight: 21
url: /hi/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Represents helper class with user-friednly interface to with AttributeSet.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | एक मान सेट करता है जो दर्शाता है कि दस्तावेज़ क्रमबद्ध है या नहीं। |
| [setCopies(int value)](#setCopies-int-) | छापे जाने वाली प्रतियों की संख्या सेट करता है। |
| [setDuplex(boolean value)](#setDuplex-boolean-) | डबल-साइड प्रिंटिंग के लिए प्रिंटर सेटिंग सेट करता है। |
| [setLandscape(boolean value)](#setLandscape-boolean-) | पृष्ठ की अभिविन्यास सेट करता है। |
| [setPrintRange(int page)](#setPrintRange-int-) | छापे जाने वाले एकल पृष्ठ को सेट करता है। |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | छापे जाने वाली पृष्ठ सीमा सेट करता है। |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | उपयोग किए जाने वाले प्रिंटर का नाम। |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | उपयोग किए जाने वाले प्रिंटर का नाम। |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। डिफ़ॉल्ट रूप से दस्तावेज़ के सभी पृष्ठ प्रिंट होते हैं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| प्रतियां | int | प्रिंट किए जाने वाले दस्तावेज़ की प्रतियों की संख्या। |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। डिफ़ॉल्ट रूप से दस्तावेज़ के सभी पृष्ठ प्रिंट होते हैं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | प्रिंटर का नाम। |
| प्रतियां | int | प्रिंट किए जाने वाले दस्तावेज़ की प्रतियों की संख्या। |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। डिफ़ॉल्ट रूप से प्रत्येक पृष्ठ की केवल एक ही प्रतिलिपि होती है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | प्रिंटर का नाम। |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


एक नया `DocumentPrintAttributeSet` उदाहरण प्रारंभ करता है। डिफ़ॉल्ट रूप से प्रत्येक पृष्ठ की केवल एक ही प्रतिलिपि होती है।

### getCopies() {#getCopies--}
```
public int getCopies()
```




**Returns:**
int
### getLandscape() {#getLandscape--}
```
public boolean getLandscape()
```




**Returns:**
boolean
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```




**Returns:**
java.lang.String
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि दस्तावेज़ क्रमबद्ध है या नहीं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true SheetCollate.COLLATED सेटिंग के बराबर है, false SheetCollate.UNCOLLATED सेटिंग के बराबर है। |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


छापे जाने वाली प्रतियों की संख्या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | प्रिंट की जाने वाली प्रतियों की संख्या। |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


डबल-साइड प्रिंटिंग के लिए प्रिंटर सेटिंग सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true Sides.DUPLEX सेटिंग के बराबर है, false Sides.ONE\\_SIDED सेटिंग के बराबर है। |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


पृष्ठ की अभिविन्यास सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true OrientationRequested.LANDSCAPE सेटिंग के बराबर है, false OrientationRequested.PORTRAIT सेटिंग के बराबर है। |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


छापे जाने वाले एकल पृष्ठ को सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | int | प्रिंट किया जाने वाला पृष्ठ। |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


छापे जाने वाली पृष्ठ सीमा सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| से | int | पहला पृष्ठ। |
| तक | int | अंतिम पृष्ठ। |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


उपयोग किए जाने वाले प्रिंटर का नाम।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | प्रिंटर का नाम। |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


उपयोग किए जाने वाले प्रिंटर का नाम।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | प्रिंटर का नाम। |
| स्थानीय | java.util.Locale | printerName का स्थानीय सेटिंग। |

