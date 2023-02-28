---
title: Class CompositeNodeBase
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.CompositeNodeBase 수업. 다른 노드를 포함할 수 있는 노드에 대한 비제네릭 클래스입니다.
type: docs
weight: 30
url: /ko/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

다른 노드를 포함할 수 있는 노드에 대한 비제네릭 클래스입니다.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 이 노드가 복합인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드에 하위 노드가 있을 수 있습니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | 노드 유형별로 모든 하위 노드를 가져옵니다. |

### 또한보십시오

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


