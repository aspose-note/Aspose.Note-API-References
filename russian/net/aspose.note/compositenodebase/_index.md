---
title: Class CompositeNodeBase
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.CompositeNodeBase сорт. Необщий класс для узлов которые могут содержать другие узлы.
type: docs
weight: 30
url: /ru/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

Необщий класс для узлов, которые могут содержать другие узлы.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Получает документ узла. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Получает значение, указывающее, является ли этот узел составным. Если true, узел может иметь дочерние узлы. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Получает следующий узел на том же уровне дерева узлов. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Получает тип узла. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Получает родительский узел. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Получает предыдущий узел на том же уровне дерева узлов. |

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Принимает посетителя узла. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Получить все дочерние узлы по типу узла. |

### Смотрите также

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


