---
title: Class DocumentVisitor
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.DocumentVisitor sınıf. Belirtilen düğümde kök ile alt ağaçta yineleme yapmak için soyut sınıf.
type: docs
weight: 70
url: /tr/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

Belirtilen düğümde kök ile alt ağaçta yineleme yapmak için soyut sınıf.

```csharp
public abstract class DocumentVisitor
```

## yöntemler

| İsim | Tanım |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Ziyaret etmek için son[`AttachedFile`](../attachedfile/) düğüm. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Ziyaret etmeye başlayın[`AttachedFile`](../attachedfile/) düğüm. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Ziyaret etmek için son[`Document`](../document/) düğüm. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Ziyaret etmeye başlayın[`Document`](../document/) düğüm. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Ziyaret etmek için son[`Image`](../image/) düğüm. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Ziyaret etmeye başlayın[`Image`](../image/) düğüm. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Ziyaret etmek için son[`OutlineElement`](../outlineelement/) düğüm. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Ziyaret etmeye başlayın[`OutlineElement`](../outlineelement/) düğüm. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Ziyaret etmek için son[`Outline`](../outline/) düğüm. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Ziyaret etmek için son[`OutlineGroup`](../outlinegroup/) düğüm. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Ziyaret etmeye başlayın[`OutlineGroup`](../outlinegroup/) düğüm. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Ziyaret etmeye başlayın[`Outline`](../outline/) düğüm. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Ziyaret etmek için son[`Page`](../page/) düğüm. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Ziyaret etmeye başlayın[`Page`](../page/) düğüm. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Ziyaret etmek için son[`RichText`](../richtext/) düğüm. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Ziyaret etmeye başlayın[`RichText`](../richtext/) düğüm. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Ziyaret etmek için son[`TableCell`](../tablecell/) düğüm. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Ziyaret etmeye başlayın[`TableCell`](../tablecell/) düğüm. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Ziyaret etmek için son[`Table`](../table/) düğüm. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Ziyaret etmek için son[`TableRow`](../tablerow/) düğüm. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Ziyaret etmeye başlayın[`TableRow`](../tablerow/) düğüm. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Ziyaret etmeye başlayın[`Table`](../table/) düğüm. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Ziyaret etmek için son[`Title`](../title/) düğüm. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Ziyaret etmeye başlayın[`Title`](../title/) düğüm. |

### Örnekler

Ziyaretçi kullanarak bir belgenin içeriğine nasıl erişileceğini gösterir.

```csharp
public static void Run()
{
    // Belgeler dizininin yolu.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Dönüştürmek istediğimiz belgeyi açın.
    Document doc = new Document(dataDir + "Aspose.one");

    // DocumentVisitor sınıfından miras alan bir nesne oluşturun.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Bu, iyi bilinen Ziyaretçi modelidir. Modelin bir ziyaretçiyi kabul etmesini sağlayın.
    // Model, karşılık gelen yöntemleri çağırarak kendi içinde yinelenir
    // ziyaretçi nesnesinde (buna ziyaret denir).
    //
    // Nesne modelindeki her düğümün Kabul yöntemine sahip olduğuna dikkat edin, böylece ziyaret
    // sadece tüm belge için değil, belgedeki herhangi bir düğüm için yürütülebilir.
    doc.Accept(myConverter);

    // Ziyaret tamamlandığında işlemin sonucunu alabiliriz,
    // bu örnekte ziyaretçide birikmiş olan.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Bir belgeyi düz metin biçiminde kaydetmenin basit uygulaması. Ziyaretçi olarak uygulandı.
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
    /// Ziyaretçi tarafından toplanan belgenin düz metnini alır.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    ///Mevcut çıktıya metin ekler. Etkin/devre dışı çıkış bayrağını onurlandırır.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Belgede bir RichText düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Belgede bir Belge düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Belgede bir Sayfa düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Bir Sayfa düğümünün işlenmesi bittiğinde çağrılır.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Belgede bir Başlık düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Belgede bir Görüntü düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Belgede bir OutlineGroup düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Belgede bir Ana Hat düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Belgede bir OutlineElement düğümüyle karşılaşıldığında çağrılır.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Ziyaretçi tarafından toplam düğüm sayısını alır
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

### Ayrıca bakınız

* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


