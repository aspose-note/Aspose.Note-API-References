---
title: Class CompositeNodeT
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.CompositeNode1T 수업. 다른 노드를 포함할 수 있는 노드의 기본 일반 클래스입니다.
type: docs
weight: 40
url: /ko/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

다른 노드를 포함할 수 있는 노드의 기본 일반 클래스입니다.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| 모수 | 설명 |
| --- | --- |
| T | 복합 노드의 요소 유형입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | 이 노드의 첫 번째 하위 노드를 가져옵니다. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | 노드가 복합인지 확인합니다. 참이면 노드에 하위 노드가 있을 수 있습니다. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | 이 노드의 마지막 하위 노드를 가져옵니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | 이 노드의 자식 노드 목록 앞에 노드를 추가합니다. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | 이 노드의 하위 노드 목록 끝에 노드를 추가합니다. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | 노드 유형별로 모든 하위 노드를 가져옵니다. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | 의 자식 노드를 반복하는 열거자를 반환합니다.`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | 이 노드에 대한 하위 노드 목록의 지정된 위치에 노드를 삽입합니다. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | 이 노드에 대한 자식 노드 목록의 지정된 위치에서 시작하는 노드의 시퀀스를 삽입합니다. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | 이 노드에 대한 자식 노드 목록의 지정된 위치에서 시작하는 노드의 시퀀스를 삽입합니다. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | 자식 노드를 제거합니다. |

### 또한보십시오

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


