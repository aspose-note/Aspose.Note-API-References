---
title: Class CompositeNodeT
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.CompositeNode1T कक्ष. नड्स के लए आधर समन्य वर्ग जसमें अन्य नड्स ह सकते हैं
type: docs
weight: 40
url: /hi/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

नोड्स के लिए आधार सामान्य वर्ग जिसमें अन्य नोड्स हो सकते हैं।

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| पैरामीटर | विवरण |
| --- | --- |
| T | समग्र नोड में तत्वों का प्रकार। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | इस नोड का पहला चाइल्ड नोड प्राप्त करता है। |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | जांचता है कि नोड समग्र है या नहीं। अगर सही है तो नोड में चाइल्ड नोड हो सकते हैं. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | इस नोड का अंतिम चाइल्ड नोड प्राप्त करता है। |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | इस नोड के लिए चाइल्ड नोड्स की सूची के सामने नोड जोड़ता है। |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | इस नोड के लिए चाइल्ड नोड्स की सूची के अंत में नोड जोड़ता है। |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | नोड प्रकार द्वारा सभी चाइल्ड नोड प्राप्त करें. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | एक एन्यूमरेटर लौटाता है जो चाइल्ड नोड के माध्यम से पुनरावृति करता है`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | नोड को इस नोड के लिए चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान पर सम्मिलित करता है। |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | इस नोड के लिए चाइल्ड नोड्स की सूची में निर्दिष्ट स्थिति से शुरू होने वाले नोड के अनुक्रम को सम्मिलित करता है। |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | इस नोड के लिए चाइल्ड नोड्स की सूची में निर्दिष्ट स्थिति से शुरू होने वाले नोड के अनुक्रम को सम्मिलित करता है। |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | चाइल्ड नोड निकालता है. |

### यह सभी देखें

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


