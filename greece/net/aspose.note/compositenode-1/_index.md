---
title: Class CompositeNodeT
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.CompositeNode1T τάξη. Η βασική γενική κλάση για κόμβους που μπορούν να περιέχουν άλλους κόμβους.
type: docs
weight: 40
url: /el/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

Η βασική γενική κλάση για κόμβους που μπορούν να περιέχουν άλλους κόμβους.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος των στοιχείων στον σύνθετο κόμβο. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Λαμβάνει τον πρώτο θυγατρικό κόμβο αυτού του κόμβου. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Ελέγχει εάν ο κόμβος είναι σύνθετος. Εάν ισχύει, τότε ο κόμβος μπορεί να έχει θυγατρικούς κόμβους. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Λαμβάνει τον τελευταίο θυγατρικό κόμβο αυτού του κόμβου. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Αποδέχεται τον επισκέπτη του κόμβου. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Προσθέτει τον κόμβο στο μπροστινό μέρος της λίστας θυγατρικών κόμβων για αυτόν τον κόμβο. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Προσθέτει τον κόμβο στο τέλος της λίστας θυγατρικών κόμβων για αυτόν τον κόμβο. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Λήψη όλων των θυγατρικών κόμβων ανά τύπο κόμβου. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Επιστρέφει έναν απαριθμητή που επαναλαμβάνεται μέσω θυγατρικών κόμβων του`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Εισάγει τον κόμβο στην καθορισμένη θέση στη λίστα θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Εισάγει την ακολουθία του κόμβου ξεκινώντας από την καθορισμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Εισάγει την ακολουθία του κόμβου ξεκινώντας από την καθορισμένη θέση στη λίστα των θυγατρικών κόμβων για αυτόν τον κόμβο. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Αφαιρεί τον θυγατρικό κόμβο. |

### Δείτε επίσης

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


