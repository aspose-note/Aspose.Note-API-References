---
title: Class IndentatedNodeT
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.IndentatedNode1T kelas. Kelas dasar untuk node dengan indentasi relatif untuk node turunan.
type: docs
weight: 300
url: /id/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

Kelas dasar untuk node dengan indentasi relatif untuk node turunan.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Parameter | Keterangan |
| --- | --- |
| T | Jenis elemen dalam node komposit. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Mendapat atau mengatur posisi indentasi. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |

## Metode

| Nama | Keterangan |
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

### Lihat juga

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


