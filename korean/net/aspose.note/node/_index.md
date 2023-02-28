---
title: Class Node
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Node 수업. Aspose.Note 문서의 모든 노드에 대한 기본 클래스.
type: docs
weight: 360
url: /ko/net/aspose.note/node/
---
## Node class

Aspose.Note 문서의 모든 노드에 대한 기본 클래스.

```csharp
public abstract class Node : INode
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

### 또한보십시오

* interface [INode](../inode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


