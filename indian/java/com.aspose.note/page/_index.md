---
title: "Page"
second_title: "Aspose.Note for Java API Reference"
description: "Represents a page."
type: docs
weight: 69
url: /hi/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Represents a page.
## Constructors

| Constructor | Description |
| --- | --- |
| [Page()](#Page--) | `Page` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [deepClone()](#deepClone--) | पृष्ठ की प्रतिलिपि बनाता है। |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | पृष्ठ की प्रतिलिपि बनाता है। |
| [getAuthor()](#getAuthor--) | लेखक को प्राप्त करता है या सेट करता है। |
| [getBackgroundColor()](#getBackgroundColor--) | पृष्ठ की बैकग्राउंड रंग को प्राप्त करता है या सेट करता है। |
| [getCreationTime()](#getCreationTime--) | निर्माण समय प्राप्त करता है या सेट करता है। |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getLevel()](#getLevel--) | स्तर को प्राप्त करता है या सेट करता है। |
| [getMargin()](#getMargin--) | मार्जिन को प्राप्त करता है या सेट करता है। |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | पृष्ठ और उसके चाइल्ड नोड्स के लिए रिवीजन सारांश को प्राप्त करता है या सेट करता है। |
| [getPageLayoutSize()](#getPageLayoutSize--) | एडिटर में प्रदर्शित पृष्ठ के लेआउट आकार को प्राप्त करता है। |
| [getSizeType()](#getSizeType--) | पृष्ठ के आकार प्रकार को प्राप्त करता है या सेट करता है। |
| [getTitle()](#getTitle--) | शीर्षक को प्राप्त करता है या सेट करता है। |
| [isConflictPage()](#isConflictPage--) | यह निर्धारित करने वाला मान प्राप्त करता है या सेट करता है कि यह पृष्ठ संघर्ष पृष्ठ है या नहीं। |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | लेखक को प्राप्त करता है या सेट करता है। |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | पृष्ठ की बैकग्राउंड रंग को प्राप्त करता है या सेट करता है। |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | यह निर्धारित करने वाला मान प्राप्त करता है या सेट करता है कि यह पृष्ठ संघर्ष पृष्ठ है या नहीं। |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | निर्माण समय प्राप्त करता है या सेट करता है। |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setLevel(byte value)](#setLevel-byte-) | स्तर को प्राप्त करता है या सेट करता है। |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | मार्जिन को प्राप्त करता है या सेट करता है। |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | पृष्ठ और उसके चाइल्ड नोड्स के लिए रिवीजन सारांश को प्राप्त करता है या सेट करता है। |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | संपादक में प्रदर्शित पृष्ठ की लेआउट आकार सेट करता है। |
| [setSizeType(int value)](#setSizeType-int-) | पृष्ठ के आकार प्रकार को प्राप्त करता है या सेट करता है। |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | शीर्षक को प्राप्त करता है या सेट करता है। |
### Page() {#Page--}
```
public Page()
```


`Page` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


पृष्ठ की प्रतिलिपि बनाता है।

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


पृष्ठ की प्रतिलिपि बनाता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cloneHistory | boolean | निर्दिष्ट करता है कि पृष्ठ का इतिहास क्लोन किया जाना चाहिए.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


लेखक को प्राप्त करता है या सेट करता है।

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


पृष्ठ की बैकग्राउंड रंग को प्राप्त करता है या सेट करता है।

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


निर्माण समय प्राप्त करता है या सेट करता है।

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


स्तर को प्राप्त करता है या सेट करता है।

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


मार्जिन को प्राप्त करता है या सेट करता है।

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


पृष्ठ और उसके चाइल्ड नोड्स के लिए रिवीजन सारांश को प्राप्त करता है या सेट करता है।

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


एडिटर में प्रदर्शित पृष्ठ के लेआउट आकार को प्राप्त करता है।

--------------------

यह मान Microsoft OneNote एप्लिकेशन द्वारा दस्तावेज़ खोलते समय अंतर्निहित पृष्ठ लेआउट प्रदर्शित करने के लिए उपयोग किया जाता है। यह दस्तावेज़ की प्रिंटिंग और सहेजने को किसी भी तरह प्रभावित नहीं करता। जब Page.SizeType प्रॉपर्टी को PageSizeType.SizeByContent पर सेट किया जाता है, तो यह प्रॉपर्टी सामग्री का वास्तविक आकार लौटाती है।

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


पृष्ठ के आकार प्रकार को प्राप्त करता है या सेट करता है।

--------------------

डिफ़ॉल्ट रूप से, पृष्ठ स्वतः आकार बदलता है। डिफ़ॉल्ट मान है [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


शीर्षक को प्राप्त करता है या सेट करता है।

मान: `Title`।

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


यह निर्धारित करने वाला मान प्राप्त करता है या सेट करता है कि यह पृष्ठ संघर्ष पृष्ठ है या नहीं।

--------------------

जब दो उपयोगकर्ता एक ही सामग्री को अपडेट करने का प्रयास करते हैं तो संघर्ष पृष्ठ उत्पन्न होता है। इस स्थिति में पहले उपयोगकर्ता के परिवर्तन सामान्य रूप से लिखे जाते हैं। लेकिन दूसरे उपयोगकर्ता के परिवर्तन मिल नहीं सकते। इसलिए पृष्ठ की केवल एक प्रति बनाई जाती है और उसे संघर्ष के रूप में चिह्नित किया जाता है।

इस संस्करण में संघर्षों को पहले उपयोगकर्ता के परिवर्तनों के पक्ष में हल किया जाता है। इसलिए यदि दस्तावेज़ में संघर्ष पृष्ठ हैं तो वे इतिहास में दिखाए जाएंगे लेकिन सहेजते समय उन्हें छोड़ दिया जाएगा। इस फ़्लैग को रीसेट करके इन पृष्ठों को सामान्य पृष्ठों की तरह इतिहास में सहेजा जा सकता है।

संघर्ष पृष्ठ को संभालने के विस्तृत उदाहरण ऑनलाइन दस्तावेज़ीकरण में पाए जा सकते हैं।

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


लेखक को प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


पृष्ठ की बैकग्राउंड रंग को प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


यह निर्धारित करने वाला मान प्राप्त करता है या सेट करता है कि यह पृष्ठ संघर्ष पृष्ठ है या नहीं।

--------------------

जब दो उपयोगकर्ता एक ही सामग्री को अपडेट करने का प्रयास करते हैं तो संघर्ष पृष्ठ उत्पन्न होता है। इस स्थिति में पहले उपयोगकर्ता के परिवर्तन सामान्य रूप से लिखे जाते हैं। लेकिन दूसरे उपयोगकर्ता के परिवर्तन मिल नहीं सकते। इसलिए पृष्ठ की केवल एक प्रति बनाई जाती है और उसे संघर्ष के रूप में चिह्नित किया जाता है।

इस संस्करण में संघर्षों को पहले उपयोगकर्ता के परिवर्तनों के पक्ष में हल किया जाता है। इसलिए यदि दस्तावेज़ में संघर्ष पृष्ठ हैं तो वे इतिहास में दिखाए जाएंगे लेकिन सहेजते समय उन्हें छोड़ दिया जाएगा। इस फ़्लैग को रीसेट करके इन पृष्ठों को सामान्य पृष्ठों की तरह इतिहास में सहेजा जा सकता है।

संघर्ष पृष्ठ को संभालने के विस्तृत उदाहरण ऑनलाइन दस्तावेज़ीकरण में पाए जा सकते हैं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


निर्माण समय प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


स्तर को प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


मार्जिन को प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


पृष्ठ और उसके चाइल्ड नोड्स के लिए रिवीजन सारांश को प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


संपादक में प्रदर्शित पृष्ठ की लेआउट आकार सेट करता है।

--------------------

यह मान Microsoft OneNote एप्लिकेशन द्वारा दस्तावेज़ खोलते समय अंतर्निहित पृष्ठ लेआउट प्रदर्शित करने के लिए उपयोग किया जाता है। यह दस्तावेज़ की प्रिंटिंग और सहेजने को किसी भी तरह प्रभावित नहीं करता। जब Page.SizeType प्रॉपर्टी को PageSizeType.SizeByContent पर सेट किया जाता है, तो यह प्रॉपर्टी सामग्री का वास्तविक आकार लौटाती है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


पृष्ठ के आकार प्रकार को प्राप्त करता है या सेट करता है।

--------------------

डिफ़ॉल्ट रूप से, पृष्ठ स्वतः आकार बदलता है। डिफ़ॉल्ट मान है [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


शीर्षक को प्राप्त करता है या सेट करता है।

मान: `Title`।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

