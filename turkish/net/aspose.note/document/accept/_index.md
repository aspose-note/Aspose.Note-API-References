---
title: Accept
second_title: Aspose.Note for .NET API Referansı
description: Düğümün ziyaretçisini kabul eder.
type: docs
weight: 80
url: /tr/net/aspose.note/document/accept/
---
## Document.Accept method

Düğümün ziyaretçisini kabul eder.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| visitor | DocumentVisitor | Şundan türetilen bir sınıfın nesnesi[`DocumentVisitor`](../../documentvisitor) . |

### Örnekler

Ziyaretçi kullanarak bir belgenin içeriğine nasıl erişileceğini gösterir.

```csharp
public static void Run()
{
    // Belgeler dizininin yolu.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Dönüştürmek istediğimiz belgeyi açıyoruz.
    Document doc = new Document(dataDir + "Aspose.one");

    // DocumentVisitor sınıfından miras alan bir nesne oluşturun.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Bu, iyi bilinen Ziyaretçi kalıbıdır. Bir ziyaretçiyi kabul etmek için modeli alın.
    // Model, ilgili yöntemleri çağırarak kendi içinde yinelenir
    // ziyaretçi nesnesinde (buna ziyaret denir).
    //
    // Nesne modelindeki her düğümün Kabul Et yöntemine sahip olduğuna dikkat edin, bu nedenle ziyaret
    // yalnızca belgenin tamamı için değil, belgedeki herhangi bir düğüm için yürütülebilir.
    doc.Accept(myConverter);

    // Ziyaret tamamlandıktan sonra işlemin sonucunu alabiliriz,
    // bu örnekte, ziyaretçide biriken.
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
    /// Mevcut çıktıya metin ekler. Etkin/devre dışı çıkış bayrağını onurlandırır.
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
    /// Belgede bir Outline düğümüyle karşılaşıldığında çağrılır.
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

* class [DocumentVisitor](../../documentvisitor)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->