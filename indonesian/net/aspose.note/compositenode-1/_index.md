---
title: Class CompositeNodeT
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.CompositeNode1T kelas. Kelas generik dasar untuk node yang dapat berisi node lain.
type: docs
weight: 40
url: /id/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

Kelas generik dasar untuk node yang dapat berisi node lain.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Parameter | Keterangan |
| --- | --- |
| T | Jenis elemen dalam node komposit. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Mendapat dokumen dari node. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Mendapat simpul anak pertama dari simpul ini. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Memeriksa apakah node tersebut komposit. Jika true maka node tersebut dapat memiliki node anak. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Mendapat simpul anak terakhir dari simpul ini. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Mendapat node berikutnya pada tingkat pohon node yang sama. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Mendapat tipe node. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Mendapat simpul induk. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Mendapat simpul sebelumnya pada tingkat pohon simpul yang sama. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Menerima pengunjung node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Menambahkan node ke bagian depan daftar node anak untuk node ini. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Menambahkan node ke akhir daftar node anak untuk node ini. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Dapatkan semua simpul anak berdasarkan jenis simpul. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Mengembalikan pencacah yang beralih melalui simpul anak dari`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Menyisipkan node ke posisi yang ditentukan dalam daftar node anak untuk node ini. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Menyisipkan urutan node mulai dari posisi yang ditentukan dalam daftar node anak untuk node ini. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Menyisipkan urutan node mulai dari posisi yang ditentukan dalam daftar node anak untuk node ini. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Menghapus simpul anak. |

### Lihat juga

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


