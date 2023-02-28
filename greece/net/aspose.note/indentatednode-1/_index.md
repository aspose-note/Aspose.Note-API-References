---
title: Class IndentatedNodeT
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.IndentatedNode1T τάξη. Η βασική κλάση για κόμβους με σχετική εσοχή για θυγατρικούς κόμβους.
type: docs
weight: 300
url: /el/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

Η βασική κλάση για κόμβους με σχετική εσοχή για θυγατρικούς κόμβους.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος των στοιχείων στον σύνθετο κόμβο. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Λαμβάνει ή ορίζει τη θέση εσοχής. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) |  |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;T&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params T[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Δείτε επίσης

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


