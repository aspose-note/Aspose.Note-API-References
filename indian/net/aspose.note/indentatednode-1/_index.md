---
title: Class IndentatedNodeT
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.IndentatedNode1T कक्ष. चइल्ड नड्स के सपेक्ष इंडेंटेशन वले नड्स के लए बेस क्लस
type: docs
weight: 300
url: /hi/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

चाइल्ड नोड्स के सापेक्ष इंडेंटेशन वाले नोड्स के लिए बेस क्लास।

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| पैरामीटर | विवरण |
| --- | --- |
| T | समग्र नोड में तत्वों का प्रकार। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | इंडेंट स्थिति प्राप्त या सेट करता है। |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
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

### यह सभी देखें

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


