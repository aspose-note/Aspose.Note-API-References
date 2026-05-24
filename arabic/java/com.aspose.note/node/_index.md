---
title: "العقدة"
second_title: "مرجع Aspose.Note for Java API"
description: "الفئة الأساسية لجميع عقد مستند **Aspose.Note**."
type: docs
weight: 51
url: /ar/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

الفئة الأساسية لجميع عقد مستند **Aspose.Note**.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getDocument()](#getDocument--) | يحصل على مستند العقدة. |
| [getNextSibling()](#getNextSibling--) | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [getNodeId()](#getNodeId--) | يحصل على معرّف العقدة. |
| [getNodeType()](#getNodeType--) | يحصل على نوع العقدة. |
| [getParentNode()](#getParentNode--) | يحصل على العقدة الأصلية. |
| [getPreviousSibling()](#getPreviousSibling--) | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |
| [isComposite()](#isComposite--) | يحصل على قيمة تشير إلى ما إذا كان هذا العنصر مركبًا. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


يحصل على مستند العقدة.

القيمة: المستند.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


يحصل على العقدة التالية في نفس مستوى شجرة العقد.

القيمة: الأخ التالي.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


يحصل على معرّف العقدة.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


يحصل على نوع العقدة.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


يحصل على العقدة الأصلية.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


يحصل على العقدة السابقة في نفس مستوى شجرة العقد.

القيمة: الأخ السابق.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


يحصل على قيمة تشير إلى ما إذا كان هذا العنصر مركبًا. إذا كان صحيحًا يمكن للعنصر أن يحتوي على عقد فرعية.

**Returns:**
boolean
