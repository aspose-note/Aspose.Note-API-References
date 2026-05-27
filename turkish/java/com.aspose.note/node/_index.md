---
title: "Düğüm"
second_title: "Aspose.Note for Java API Referansı"
description: "Aspose.Note belgesindeki tüm düğümler için temel sınıf."
type: docs
weight: 51
url: /tr/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Aspose.Note belgesindeki tüm düğümler için temel sınıf.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getDocument()](#getDocument--) | Düğümün belgesini alır. |
| [getNextSibling()](#getNextSibling--) | Aynı düğüm ağacı seviyesindeki sonraki düğümü alır. |
| [getNodeId()](#getNodeId--) | Düğümün kimliğini alır. |
| [getNodeType()](#getNodeType--) | Düğüm türünü alır. |
| [getParentNode()](#getParentNode--) | Üst düğümü alır. |
| [getPreviousSibling()](#getPreviousSibling--) | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |
| [isComposite()](#isComposite--) | Bu düğümün birleşik olup olmadığını gösteren bir değeri alır. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Düğümün belgesini alır.

Değer: Belge.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Aynı düğüm ağacı seviyesindeki sonraki düğümü alır.

Değer: Sonraki kardeş.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Düğümün kimliğini alır.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Düğüm türünü alır.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Üst düğümü alır.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Aynı düğüm ağacı seviyesindeki önceki düğümü alır.

Değer: Önceki kardeş.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Bu düğümün birleşik olup olmadığını gösteren bir değeri alır. Doğru ise düğüm alt düğümlere sahip olabilir.

**Returns:**
boolean
