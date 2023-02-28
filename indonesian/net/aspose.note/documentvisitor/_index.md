---
title: Class DocumentVisitor
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.DocumentVisitor kelas. Kelas abstrak untuk iterasi melalui subtree dengan root pada node yang ditentukan.
type: docs
weight: 70
url: /id/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

Kelas abstrak untuk iterasi melalui subtree dengan root pada node yang ditentukan.

```csharp
public abstract class DocumentVisitor
```

## Metode

| Nama | Keterangan |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Selesai untuk mengunjungi[`AttachedFile`](../attachedfile/) simpul. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Mulai mengunjungi[`AttachedFile`](../attachedfile/) simpul. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Selesai untuk mengunjungi[`Document`](../document/) simpul. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Mulai mengunjungi[`Document`](../document/) simpul. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Selesai untuk mengunjungi[`Image`](../image/) simpul. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Mulai mengunjungi[`Image`](../image/) simpul. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Selesai untuk mengunjungi[`OutlineElement`](../outlineelement/) simpul. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Mulai mengunjungi[`OutlineElement`](../outlineelement/) simpul. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Selesai untuk mengunjungi[`Outline`](../outline/) simpul. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Selesai untuk mengunjungi[`OutlineGroup`](../outlinegroup/) simpul. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Mulai mengunjungi[`OutlineGroup`](../outlinegroup/) simpul. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Mulai mengunjungi[`Outline`](../outline/) simpul. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Selesai untuk mengunjungi[`Page`](../page/) simpul. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Mulai mengunjungi[`Page`](../page/) simpul. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Selesai untuk mengunjungi[`RichText`](../richtext/) simpul. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Mulai mengunjungi[`RichText`](../richtext/) simpul. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Selesai untuk mengunjungi[`TableCell`](../tablecell/) simpul. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Mulai mengunjungi[`TableCell`](../tablecell/) simpul. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Selesai untuk mengunjungi[`Table`](../table/) simpul. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Selesai untuk mengunjungi[`TableRow`](../tablerow/) simpul. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Mulai mengunjungi[`TableRow`](../tablerow/) simpul. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Mulai mengunjungi[`Table`](../table/) simpul. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Selesai untuk mengunjungi[`Title`](../title/) simpul. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Mulai mengunjungi[`Title`](../title/) simpul. |

### Contoh

Menunjukkan cara mengakses konten dokumen menggunakan pengunjung.

```csharp
public static void Run()
{
    // Jalur ke direktori dokumen.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Buka dokumen yang ingin kita konversi.
    Document doc = new Document(dataDir + "Aspose.one");

    // Buat objek yang mewarisi dari kelas DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Ini adalah pola Pengunjung yang terkenal. Dapatkan model untuk menerima pengunjung.
    // Model akan melakukan iterasi sendiri dengan memanggil metode yang sesuai
    // pada objek pengunjung (ini disebut mengunjungi).
    //
    // Perhatikan bahwa setiap node dalam model objek memiliki metode Terima sehingga kunjungan
    // dapat dieksekusi tidak hanya untuk seluruh dokumen, tetapi untuk setiap node dalam dokumen.
    doc.Accept(myConverter);

    // Setelah kunjungan selesai, kita dapat mengambil hasil operasi,
    // yang dalam contoh ini, telah terkumpul di pengunjung.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Implementasi sederhana untuk menyimpan dokumen dalam format teks biasa. Diimplementasikan sebagai Pengunjung.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// Mendapat teks biasa dari dokumen yang dikumpulkan oleh pengunjung.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Menambahkan teks ke output saat ini. Menghormati bendera keluaran yang diaktifkan/dinonaktifkan.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Dipanggil ketika node RichText ditemui dalam dokumen.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Dipanggil ketika simpul Dokumen ditemui dalam dokumen.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Dipanggil saat simpul Halaman ditemui dalam dokumen.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Dipanggil saat pemrosesan simpul Halaman selesai.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Dipanggil ketika simpul Judul ditemui dalam dokumen.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Dipanggil ketika simpul Gambar ditemui dalam dokumen.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Dipanggil ketika simpul OutlineGroup ditemui dalam dokumen.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Dipanggil saat node Outline ditemukan dalam dokumen.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Dipanggil saat node OutlineElement ditemui di dokumen.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Mendapatkan jumlah total node oleh Pengunjung
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### Lihat juga

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


