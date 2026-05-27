---
title: "الفئة CompositeNodeBase"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.CompositeNodeBase. الفئة غير العامة للعقد التي يمكنها احتواء عقد أخرى"
type: docs
weight: 30
url: /ar/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

الفئة غير العامة للعقد التي يمكنها احتواء عقد أخرى.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كانت true يمكن للعقدة أن تحتوي على عقد فرعية. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | احصل على جميع عقد الطفل حسب نوع العقدة. |

### انظر أيضًا

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


