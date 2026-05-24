---
title: "CompositeNode"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Η βασική γενική κλάση για κόμβους που μπορούν να περιέχουν άλλους κόμβους."
type: docs
weight: 15
url: /el/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

Η βασική γενική κλάση για κόμβους που μπορούν να περιέχουν άλλους κόμβους.

`T`: Ο τύπος των στοιχείων στον σύνθετο κόμβο.

T :
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Προσθέτει τον κόμβο στην αρχή της λίστας των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Προσθέτει τον κόμβο στο τέλος της λίστας των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Λαμβάνει όλους τους κόμβους-παιδιά με βάση τον τύπο του κόμβου. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Εισάγει τον κόμβο στη συγκεκριμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Αφαιρεί τον κόμβο-παιδί. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getFirstChild()](#getFirstChild--) | Αποκτά τον πρώτο θυγατρικό κόμβο αυτού του κόμβου. |
| [getLastChild()](#getLastChild--) | Αποκτά τον τελευταίο θυγατρικό κόμβο αυτού του κόμβου. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Εισάγει τη σειρά των κόμβων αρχίζοντας από τη συγκεκριμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Εισάγει τη σειρά των κόμβων αρχίζοντας από τη συγκεκριμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [isComposite()](#isComposite--) | Ελέγχει αν ο κόμβος είναι σύνθετος. |
| [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη που διατρέχει τους θυγατρικούς κόμβους του `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Προσθέτει τον κόμβο στην αρχή της λίστας των θυγατρικών κόμβων για αυτόν τον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newChild | T1 | Ο κόμβος προς προσθήκη. |

**Returns:**
T1 - Ο προστιθέμενος κόμβος.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Προσθέτει τον κόμβο στο τέλος της λίστας των θυγατρικών κόμβων για αυτόν τον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newChild | T1 | Ο κόμβος προς προσθήκη. |

**Returns:**
T1 - Ο προστιθέμενος κόμβος.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Λαμβάνει όλους τους κόμβους-παιδιά με βάση τον τύπο του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Μια λίστα παιδικών κόμβων.

`T1`: Ο τύπος των στοιχείων στη επιστρεφόμενη λίστα.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Εισάγει τον κόμβο στη συγκεκριμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| i | int | Θέση για εισαγωγή |
| newChild | T1 | Ο κόμβος για εισαγωγή. |

**Returns:**
T1 - Ο προστιθέμενος κόμβος.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Αφαιρεί τον κόμβο-παιδί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldChild | T1 | Ο κόμβος προς αφαίρεση. |

**Returns:**
T1 - Ο αφαιρεμένος κόμβος.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Αποκτά τον πρώτο θυγατρικό κόμβο αυτού του κόμβου.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Αποκτά τον τελευταίο θυγατρικό κόμβο αυτού του κόμβου.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Εισάγει τη σειρά των κόμβων αρχίζοντας από τη συγκεκριμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| i | int | Θέση για εισαγωγή |
| newChildren | T[] | Η σειρά των κόμβων που θα εισαχθούν. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Εισάγει τη σειρά των κόμβων αρχίζοντας από τη συγκεκριμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| i | int | Θέση για εισαγωγή |
| newChildren | java.lang.Iterable&lt;T&gt; | Η σειρά των κόμβων που θα εισαχθούν. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Ελέγχει εάν ο κόμβος είναι σύνθετος. Εάν είναι αληθές, τότε ο κόμβος μπορεί να έχει υποκόμβους.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Επιστρέφει έναν επαναλήπτη που διατρέχει τους θυγατρικούς κόμβους του `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Ένα `T:IEnumerator`1` για το `CompositeNode\{T\}`.
