---
title: "Node"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Η βασική κλάση για όλους τους κόμβους ενός εγγράφου Aspose.Note."
type: docs
weight: 51
url: /el/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Η βασική κλάση για όλους τους κόμβους ενός εγγράφου Aspose.Note.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getDocument()](#getDocument--) | Λαμβάνει το έγγραφο του κόμβου. |
| [getNextSibling()](#getNextSibling--) | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβων. |
| [getNodeId()](#getNodeId--) | Λαμβάνει το αναγνωριστικό του κόμβου. |
| [getNodeType()](#getNodeType--) | Λαμβάνει τον τύπο του κόμβου. |
| [getParentNode()](#getParentNode--) | Λαμβάνει τον γονικό κόμβο. |
| [getPreviousSibling()](#getPreviousSibling--) | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβων. |
| [isComposite()](#isComposite--) | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο κόμβος είναι σύνθετος. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Λαμβάνει το έγγραφο του κόμβου.

Τιμή: Το έγγραφο.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβων.

Τιμή: Ο επόμενος αδελφός.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Λαμβάνει το αναγνωριστικό του κόμβου.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Λαμβάνει τον τύπο του κόμβου.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Λαμβάνει τον γονικό κόμβο.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβων.

Τιμή: Ο προηγούμενος αδελφός.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο κόμβος είναι σύνθετος. Εάν είναι αληθές, ο κόμβος μπορεί να έχει υποκόμβους.

**Returns:**
boolean
