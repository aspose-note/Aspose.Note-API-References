---
title: "فئة OutlineGroup"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "Aspose.Note.OutlineGroup فئة. تمثل مجموعة OutlineGroup"
type: docs
weight: 540
url: /ar/net/aspose.note/outlinegroup/
---
## OutlineGroup class

يمثل مجموعة مخطط.

```csharp
public sealed class OutlineGroup : IndentatedNode<IOutlineChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [OutlineGroup](outlinegroup/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/outlinegroup/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### انظر أيضًا

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


