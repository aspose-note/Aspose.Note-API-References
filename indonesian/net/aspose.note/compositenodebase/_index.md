---
title: Class CompositeNodeBase
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.CompositeNodeBase kelas. Kelas nongenerik untuk node yang dapat berisi node lain.
type: docs
weight: 30
url: /id/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

Kelas non-generik untuk node yang dapat berisi node lain.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Mendapat nilai yang menunjukkan apakah simpul ini komposit. Jika true node dapat memiliki node anak. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |

## Metode

| Nama | Keterangan |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Menerima pengunjung node. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Dapatkan semua simpul anak berdasarkan jenis simpul. |

### Lihat juga

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


