---
title: Class CompositeNodeBase
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.CompositeNodeBase कक्ष. नड्स के लए गैरजेनेरक वर्ग जसमें अन्य नड्स ह सकते हैं
type: docs
weight: 30
url: /hi/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

नोड्स के लिए गैर-जेनेरिक वर्ग जिसमें अन्य नोड्स हो सकते हैं।

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि यह नोड समग्र है या नहीं। यदि सही है तो नोड में चाइल्ड नोड हो सकते हैं. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | नोड प्रकार द्वारा सभी चाइल्ड नोड प्राप्त करें. |

### यह सभी देखें

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


