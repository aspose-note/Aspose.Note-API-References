---
title: Class CompositeNodeT
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.CompositeNode1T clase. La clase genérica base para nodos que pueden contener otros nodos.
type: docs
weight: 40
url: /es/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

La clase genérica base para nodos que pueden contener otros nodos.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de elementos en el nodo compuesto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Obtiene el documento del nodo. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Obtiene el primer nodo secundario de este nodo. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Comprueba si el nodo es compuesto. Si es verdadero, el nodo puede tener nodos secundarios. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Obtiene el último nodo hijo de este nodo. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtiene el siguiente nodo en el mismo nivel de árbol de nodos. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtiene el tipo de nodo. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtiene el nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtiene el nodo anterior en el mismo nivel de árbol de nodos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Acepta al visitante del nodo. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Agrega el nodo al frente de la lista de nodos secundarios para este nodo. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Agrega el nodo al final de la lista de nodos secundarios para este nodo. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Obtener todos los nodos secundarios por tipo de nodo. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Devuelve un enumerador que itera a través de los nodos secundarios del`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Inserta el nodo en la posición especificada en la lista de nodos secundarios para este nodo. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Inserta la secuencia del nodo a partir de la posición especificada en la lista de nodos secundarios para este nodo. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Inserta la secuencia del nodo a partir de la posición especificada en la lista de nodos secundarios para este nodo. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Elimina el nodo secundario. |

### Ver también

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


