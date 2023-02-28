---
title: Class IndentatedNodeT
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.IndentatedNode1T فصل. الفئة الأساسية للعقد ذات المسافة البادئة النسبية للعقد الفرعية.
type: docs
weight: 300
url: /ar/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

الفئة الأساسية للعقد ذات المسافة البادئة النسبية للعقد الفرعية.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| معامل | وصف |
| --- | --- |
| T | نوع العناصر في العقدة المركبة. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على وثيقة العقدة . |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | الحصول على موضع المسافة البادئة أو تعيينه . |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة . |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |

## طُرق

| اسم | وصف |
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

### أنظر أيضا

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


