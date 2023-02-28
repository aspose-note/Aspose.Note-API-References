---
title: Class Node
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Node сорт. Базовый класс для всех узлов документа Aspose.Note.
type: docs
weight: 360
url: /ru/net/aspose.note/node/
---
## Node class

Базовый класс для всех узлов документа Aspose.Note.

```csharp
public abstract class Node : INode
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

### Смотрите также

* interface [INode](../inode/)
* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


