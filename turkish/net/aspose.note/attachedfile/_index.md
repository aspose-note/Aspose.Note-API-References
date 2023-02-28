---
title: Class AttachedFile
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.AttachedFile sınıf. Ekli bir dosyayı temsil eder.
type: docs
weight: 10
url: /tr/net/aspose.note/attachedfile/
---
## AttachedFile class

Ekli bir dosyayı temsil eder.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | Yeni bir örneğini başlatır.`AttachedFile` sınıf. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | Yeni bir örneğini başlatır.`AttachedFile` sınıf. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | Yeni bir örneğini başlatır.`AttachedFile` sınıf. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | Yeni bir örneğini başlatır.`AttachedFile` sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | Hizalamayı alır veya ayarlar. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | Ekli dosyanın simgesi için bir gövde alternatif metni alır veya ayarlar. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | Ekli dosyanın simgesi için alternatif bir metin başlığı alır veya ayarlar. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | Katıştırılmış bir dosya için ikili verileri alır. |
| [Document](../../aspose.note/node/document/) { get; } | Düğümün belgesini alır. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | Katıştırılmış bir dosyanın uzantısını alır. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | Gömülü dosyanın adını alır. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | Orijinal dosyanın yolunu alır. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | Gömülü dosya simgesinin orijinal yüksekliğini alır. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | Yatay ofseti alır veya ayarlar. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | Katıştırılmış dosyayla ilişkili simge için ikili verileri alır. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | Simgenin uzantısını alır. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Bu düğümün bileşik olup olmadığını gösteren bir değer alır. Doğruysa, düğümün alt düğümleri olabilir. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | Dosyanın görünümünün çıktı olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | Simge boyutunun değerinin kullanıcı tarafından açıkça güncellenip güncellenmediğini gösteren bir değer alır veya ayarlar. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | Katıştırılmış dosya simgesini görüntülemek için maksimum yüksekliği alır veya ayarlar. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | Katıştırılmış dosya simgesini görüntülemek için maksimum genişliği alır veya ayarlar. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Aynı düğüm ağacı seviyesindeki bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Düğüm türünü alır. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | Bir paragrafın tüm etiketlerinin listesini alır. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | Gömülü dosyanın metin temsilini alır veya ayarlar. Dize, 10 (satır besleme) veya 13 (satır başı). değerinde herhangi bir karakter İÇERMEZ OLMALIDIR. |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | Dikey ofseti alır veya ayarlar. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | Gömülü dosya simgesinin orijinal genişliğini alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |

### Örnekler

Ekli bir dosyanın içeriğinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Sample1.one");

// Ekli dosya düğümlerinin bir listesini alın
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Tüm düğümleri yinele
foreach (AttachedFile file in nodes)
{
    // Ekli dosyayı bir akış nesnesine yükleyin
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Yerel bir dosya oluştur
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Dosya akışını kopyala
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Dosya yolunu kullanarak bir belgeye nasıl dosya ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile sınıf nesnesini başlat
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Ekli dosyayı ekle
outlineElem.AppendChildLast(attachedFile);

// Ana hat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Bir akıştan bir belgeye nasıl dosya ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // AttachedFile sınıf nesnesini başlat ve simge yolunu da ilet
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Ekli dosyayı ekle
    outlineElem.AppendChildLast(attachedFile);
}

// Ana hat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Ayrıca bakınız

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


