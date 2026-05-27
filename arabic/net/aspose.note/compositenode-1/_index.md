---
title: "الفئة CompositeNodeT"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.CompositeNode1T. الفئة العامة الأساسية للعقد التي يمكنها احتواء عقد أخرى"
type: docs
weight: 40
url: /ar/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

الفئة العامة الأساسية للعقد التي يمكنها احتواء عقد أخرى.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| معامل | الوصف |
| --- | --- |
| T | نوع العناصر في العقدة المركبة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | يحصل على العقدة الفرعية الأولى لهذه العقدة. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | يتحقق مما إذا كانت العقدة مركبة. إذا كان صحيحًا فإن العقدة يمكن أن تحتوي على عقد فرعية. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | يحصل على العقدة الفرعية الأخيرة لهذه العقدة. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | يضيف العقدة إلى مقدمة قائمة العقد الفرعية لهذه العقدة. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | يضيف العقدة إلى نهاية قائمة العقد الفرعية لهذه العقدة. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | احصل على جميع عقد الطفل حسب نوع العقدة. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | يرجع عدّادًا يتنقل عبر العقد الفرعية لـ `CompositeNode`. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | يدرج العقدة في الموضع المحدد في قائمة العقد الفرعية لهذه العقدة. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | يدرج تسلسل العقدة بدءًا من الموضع المحدد في قائمة العقد الفرعية لهذه العقدة. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | يدرج تسلسل العقدة بدءًا من الموضع المحدد في قائمة العقد الفرعية لهذه العقدة. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | يزيل عقدة الطفل. |

### انظر أيضًا

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


