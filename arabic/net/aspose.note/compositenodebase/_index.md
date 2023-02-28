---
title: Class CompositeNodeBase
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.CompositeNodeBase فصل. الفئة غير العامة للعقد التي يمكن أن تحتوي على عقد أخرى.
type: docs
weight: 30
url: /ar/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

الفئة غير العامة للعقد التي يمكن أن تحتوي على عقد أخرى.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على وثيقة العقدة . |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كان هذا صحيحًا ، يمكن أن تحتوي العقدة على عقد فرعية. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة . |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |

## طُرق

| اسم | وصف |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | يقبل زائر العقدة . |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | احصل على جميع العقد الفرعية حسب نوع العقدة . |

### أنظر أيضا

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


