---
title: "OutlineElement"
second_title: "Aspose.Note for Java API Reference"
description: "Represents a OutlineElement."
type: docs
weight: 67
url: /hi/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Represents a OutlineElement.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | `OutlineElement` क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | आउटलाइन तत्व का सबसे हालिया लेखक प्राप्त करता है। |
| [getAuthorOriginal()](#getAuthorOriginal--) | आउटलाइन तत्व का मूल लेखक प्राप्त करता है। |
| [getCreationTime()](#getCreationTime--) | निर्माण समय प्राप्त करता है या सेट करता है। |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getNumberList()](#getNumberList--) | क्रमांकित सूची शीर्षक के लिए शैली प्राप्त करता है या सेट करता है। |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | निर्माण समय प्राप्त करता है या सेट करता है। |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | क्रमांकित सूची शीर्षक के लिए शैली प्राप्त करता है या सेट करता है। |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


`OutlineElement` क्लास का एक नया उदाहरण प्रारंभ करता है।

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


आउटलाइन तत्व का सबसे हालिया लेखक प्राप्त करता है।

मान: सबसे हालिया लेखक।

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


आउटलाइन तत्व का मूल लेखक प्राप्त करता है।

मान: मूल लेखक।

**Returns:**
java.lang.String
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
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


क्रमांकित सूची शीर्षक के लिए शैली प्राप्त करता है या सेट करता है।

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
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

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


क्रमांकित सूची शीर्षक के लिए शैली प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

