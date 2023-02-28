---
title: Class CompositeNodeBase
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.CompositeNodeBase τάξη. Η μη γενική κλάση για κόμβους που μπορούν να περιέχουν άλλους κόμβους.
type: docs
weight: 30
url: /el/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

Η μη γενική κλάση για κόμβους που μπορούν να περιέχουν άλλους κόμβους.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο κόμβος είναι σύνθετος. Εάν είναι αληθές, ο κόμβος μπορεί να έχει θυγατρικούς κόμβους. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Αποδέχεται τον επισκέπτη του κόμβου. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Λήψη όλων των θυγατρικών κόμβων ανά τύπο κόμβου. |

### Δείτε επίσης

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


