---
title: Document.Accept
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. Menerima pengunjung node.
type: docs
weight: 80
url: /id/net/aspose.note/document/accept/
---
## Document.Accept method

Menerima pengunjung node.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| visitor | DocumentVisitor | Objek kelas berasal dari[`DocumentVisitor`](../../documentvisitor/) . |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


