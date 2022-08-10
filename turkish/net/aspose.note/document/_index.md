---
title: Document
second_title: Aspose.Note for .NET API Referansı
description: Bir Aspose.Note belgesini temsil eder.
type: docs
weight: 60
url: /tr/net/aspose.note/document/
---
## Document class

Bir Aspose.Note belgesini temsil eder.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Document](document#constructor)() | Yeni bir örneğini başlatır[`Document`](../document) class. Boş bir OneNote belgesi oluşturur. |
| [Document](document#constructor_1)(Stream) | Yeni bir örneğini başlatır[`Document`](../document) class. Bir akıştan mevcut bir OneNote belgesini açar. |
| [Document](document#constructor_3)(string) | Yeni bir örneğini başlatır[`Document`](../document) class. Bir dosyadan mevcut bir OneNote belgesini açar. |
| [Document](document#constructor_2)(Stream, LoadOptions) | Yeni bir örneğini başlatır[`Document`](../document) class. Bir akıştan var olan bir OneNote belgesini açar. Şifreleme parolası gibi ek seçeneklerin belirlenmesine izin verir. |
| [Document](document#constructor_4)(string, LoadOptions) | Yeni bir örneğini başlatır[`Document`](../document) class. Bir dosyadan var olan bir OneNote belgesini açar. Şifreleme parolası gibi ek seçeneklerin belirlenmesine izin verir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | Aspose.Note'un mizanpaj değişikliklerini otomatik olarak tespit edip etmediğini gösteren bir değer alır veya ayarlar. Varsayılan değer`doğru` . |
| [Color](../../aspose.note/document/color) { get; set; } | Rengi alır veya ayarlar. |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | Oluşturma zamanını alır veya ayarlar. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | Görünen adı alır veya ayarlar. |
| [Document](../../aspose.note/node/document) { get; } | Düğümün belgesini alır. |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | Dosya biçimini alır (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | Nesnenin global olarak benzersiz kimliğini alır. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Aynı düğüm ağacı düzeyinde bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Düğüm türünü alır. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Aynı düğüm ağacı düzeyinde önceki düğümü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | Bir öncekinden bu yana belge düzeninde yapılan tüm değişiklikleri algılar.[`DetectLayoutChanges`](./detectlayoutchanges) call. Duruma göre[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) true olarak ayarlanır, belge dışa aktarımının başlangıcında otomatik olarak kullanılır. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | [`PageHistory`](../pagehistory) bir belgede sunulan her sayfanın tam geçmişini içerir (en erken dizin 0'da). Geçerli sayfa revizyonuna şu şekilde erişilebilir:[`Current`](../pagehistory/current)ve geçmiş sürümler koleksiyonundan ayrı olarak bulunur. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | Sağlanan PDF belgesinden bir dizi sayfayı içe aktarır. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | Sağlanan PDF belgesinden bir dizi sayfayı içe aktarır. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | Bir dizi sayfayı belgeyle birleştirir. |
| [Print](../../aspose.note/document/print#print)() | Belgeyi varsayılan yazıcıyı kullanarak yazdırır. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | Belgeyi varsayılan yazıcıyı kullanarak yazdırır. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | OneNote belgesini bir akışa kaydeder. |
| [Save](../../aspose.note/document/save#save_3)(string) | OneNote belgesini bir dosyaya kaydeder. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | OneNote belgesini belirtilen biçimde bir akışa kaydeder. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak OneNote belgesini bir akışa kaydeder. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | OneNote belgesini belirtilen biçimde bir dosyaya kaydeder. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak OneNote belgesini bir dosyaya kaydeder. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | Bir dosyadaki belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | Bir dosyadaki belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | Bir dosyadaki belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir. |

### Örnekler

Varsayılan seçeneklerle standart Windows iletişim kutusunu kullanarak belgenin bir yazıcıya nasıl gönderileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Şifrelenmiş bir belgenin nasıl yapıldığını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Belgenin şifreleme ile nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

SaveFormat numaralandırma kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

OneSaveOptions kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Bir belgenin sayfa sayısının nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Sayfa sayısını al
int count = oneFile.Count();

// Çıktı ekranında sayıyı yazdır
Console.WriteLine(count);
```

Varsayılan ayarlar kullanılarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Bir belgenin gif biçiminde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Belgeyi gif olarak kaydedin.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Belgeyi JPEG biçiminde görüntü olarak kaydederken görüntü kalitesinin nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Belgeyi kaydedin.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Belgeyi resim olarak kaydederken bir resim çözünürlüğünün nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Belgeyi kaydedin.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Bir belgenin dosya biçiminin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010'u işle
        break;
    case FileFormat.OneNoteOnline:
        // OneNote'u Çevrimiçi İşle
        break;
}
```

Bir görüntüye bir köprünün nasıl bağlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://resim.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Bir belgenin akışa nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Bir sonraki okuyucu için hazır olması için akış konumunu sıfıra geri sarın.
dstStream.Seek(0, SeekOrigin.Begin);
```

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Bir not defterine nasıl yeni bölüm ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Defter'e yeni bir çocuk ekle
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Not Defterini Kaydet
notebook.Save(dataDir);
```

OneNote 2007 biçimi desteklenmediği için belge yüklemesinin başarısız olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

Bir sayfanın önceki sürümünün nasıl geri yükleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle ve ilk çocuğu al           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Bir sayfanın nasıl klonlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Geçmiş olmadan yeni belgeye klonla
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Geçmişi olan yeni belgeye klonla
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

Tüm kaynakları (css/fonts/images) ayrı bir dosyaya depolayarak bir belgenin html formatında nasıl kaydedileceğini gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Tüm kaynakların (css/fonts/images) gömülmesiyle bir belgenin html formatında bir akışa nasıl kaydedileceğini gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

Bir görüntü için metin açıklamasının nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Bir sayfa hakkında meta bilgilerin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Uzun OneNote sayfaları pdf biçiminde kaydedildiğinde, sayfalara bölünür. Örnek, sayfa sonlarında bulunan nesnelerin bölme mantığının nasıl yapılandırılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Bir belgenin png formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions nesnesini başlat 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Sayfa indeksini ayarla
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Belgeyi PNG olarak kaydedin.
oneFile.Save(dataDir, opts);
```

Sayfanın geçmişinin nasıl düzenleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle ve ilk çocuğu al           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

Bir not defterinin içeriğinden nasıl geçileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Alt belgeyle bir şeyler yap
        }
        else if (notebookChildNode is Notebook)
        {
            // Alt not defteriyle bir şeyler yap
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

Bir belgeden nasıl görüntü alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm Görüntü düğümlerini al
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Görüntü baytlarını bir dosyaya kaydet
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions nesnesini başlat
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Kaydedilecek ilk sayfanın sayfa indeksini ayarla
                              PageIndex = 0,

                              // Sayfa sayısını ayarla
                              PageCount = 1,
                          };

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Belirli ayarlar kullanılarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions nesnesini başlat
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Jpeg sıkıştırmasını kullan
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG sıkıştırması için kalite
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Belirtilen seçeneklerle standart Windows iletişim kutusunu kullanarak belgenin bir yazıcıya nasıl gönderileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

Resmin meta bilgilerinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm Görüntü düğümlerini al
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Ekli bir dosyanın içeriğinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Sample1.one");

// Ekli dosya düğümlerinin bir listesini alın
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Tüm düğümler arasında yineleme
foreach (AttachedFile file in nodes)
{
    // Ekli dosyayı bir akış nesnesine yükle
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // yerel bir dosya oluştur
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Dosya akışını kopyala
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Sayfanın geçmişinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// İlk sayfayı al
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

Dosya yolunu kullanarak bir belgeye nasıl dosya ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document sınıfının bir nesnesini oluşturun
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

// Anahat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Varsayılan seçenekleri kullanarak bir belgenin nasıl oluşturulacağını ve html biçiminde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote belgesini başlat
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Belgedeki tüm metinler için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// HTML biçiminde kaydet
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Bir sayfanın çakışma sayfası olup olmadığının nasıl kontrol edileceğini gösterir (yani, OneNote'un otomatik olarak birleştiremeyeceği değişikliklere sahiptir).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükle
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Varsayılan olarak çakışan sayfalar kaydedilirken atlanır.
    // Çakışmaz olarak işaretlerseniz, tarihte her zamanki gibi kaydedilecektir.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Kullanıcı tanımlı özelliklere sahip bir belgeye dosyadan nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Akıştan belge yükle.
Document doc = new Document(dataDir + "Aspose.one");

// Belgenin ilk sayfasını al.
Aspose.Note.Page page = doc.FirstChild;

// Dosyadan bir resim yükleyin.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Resmin boyutunu ihtiyaçlarınıza göre değiştirin (isteğe bağlı).
                              Width = 100,
                              Height = 100,

                              // Resmin sayfadaki konumunu ayarlayın (isteğe bağlı).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Görüntü hizalamasını ayarla
                              Alignment = HorizontalAlignment.Right
                          };

// Resmi sayfaya ekleyin.
page.AppendChildLast(image);
```

Bir akıştan bir belgeye nasıl dosya ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // AttachedFile sınıf nesnesini başlatın ve ayrıca simge yolunu iletin
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Ekli dosyayı ekle
    outlineElem.AppendChildLast(attachedFile);
}

// Anahat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Uzun OneNote sayfaları pdf biçiminde kaydedildiğinde, sayfalara bölünür. Örnek, sayfa sonlarında bulunan nesnelerin bölme mantığının nasıl yapılandırılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Bir belgenin nasıl oluşturulacağını ve belirtilen sayfa aralığının html biçiminde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote belgesini başlat
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Belgedeki tüm metinler için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML biçiminde kaydet
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Başlık sayfası olan bir belgenin nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Aspose.Note.Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Belgedeki tüm metinler için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Sayfa başlığı özelliklerini ayarla
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Belgeye Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Akıştan bir belgeye nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Görüntü adını, uzantısını ve akışını kullanarak ikinci görüntüyü yükleyin.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Görüntü hizalamasını ayarla
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Dosyadan belgeye nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat ve ofset özelliklerini ayarla
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// Dosya yoluna göre bir resim yükleyin.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Görüntü hizalamasını ayarla
                              Alignment = HorizontalAlignment.Right
                          };

// Resim eklemek
outlineElem.AppendChildLast(image);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Metin içeren bir belgenin nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Page page = new Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle sınıf nesnesini başlat ve biçimlendirme özelliklerini ayarla
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText sınıf nesnesini başlat ve metin stili uygula
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText düğümü ekle
outlineElem.AppendChildLast(text);

// OutlineElement düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Bir belgenin farklı biçimlerde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Yeni Belgeyi başlat
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Yeni Sayfayı başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Belgedeki tüm metinler için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini farklı biçimlerde kaydedin, metin yazı tipi boyutunu ayarlayın ve düzen değişikliklerini manuel olarak algılayın.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

Kullanıcı tanımlı geri aramaları kullanarak tüm kaynakları (css/fonts/images) depolayarak bir belgenin html formatında nasıl kaydedileceğini gösterir.

```csharp
// Aşağıdaki kod, document.html dosyasını içeren 'documentFolder' klasörünü, 'style.css' dosyasını içeren 'css' klasörünü, görüntüleri içeren 'images' klasörünü ve yazı tiplerini içeren 'fonts' klasörünü oluşturur.
// 'style.css' dosyasının sonunda aşağıdaki dizeyi içerecektir "/* Bu satır, kullanıcı tarafından manuel olarak akışa eklenir */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

Bir metne bir köprünün nasıl bağlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tasks();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem);

// Title sınıf nesnesini başlat
Title title = new Title() { TitleText = titleText };

// Sayfa sınıfı nesnesini başlat
Page page = new Note.Page() { Title = title };

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
