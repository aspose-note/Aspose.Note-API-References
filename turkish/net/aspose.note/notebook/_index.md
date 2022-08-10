---
title: Notebook
second_title: Aspose.Note for .NET API Referansı
description: Bir Aspose.Note not defterini temsil eder.
type: docs
weight: 390
url: /tr/net/aspose.note/notebook/
---
## Notebook class

Bir Aspose.Note not defterini temsil eder.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Notebook](notebook#constructor)() | Yeni bir örneğini başlatır[`Notebook`](../notebook) sınıf. |
| [Notebook](notebook#constructor_1)(Stream) | Yeni bir örneğini başlatır[`Notebook`](../notebook) class. Bir akıştan mevcut bir OneNote not defterini açar. |
| [Notebook](notebook#constructor_3)(string) | Yeni bir örneğini başlatır[`Notebook`](../notebook) class. Bir dosyadan mevcut bir OneNote not defterini açar. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | Yeni bir örneğini başlatır[`Notebook`](../notebook) class. Bir akıştan mevcut bir OneNote not defterini açar. Ek yükleme seçenekleri belirlemeye izin verir. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | Yeni bir örneğini başlatır[`Notebook`](../notebook)class. Bir dosyadan var olan bir OneNote not defterini açar. Alt yükleme stratejisi ("tembel"/anında) gibi ek seçeneklerin belirtilmesine izin verir. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Rengi alır veya ayarlar. |
| [Count](../../aspose.note/notebook/count) { get; } | İçinde bulunan öğelerin sayısını alır[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Görünen adı alır veya ayarlar. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Dosya biçimini alır (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Nesnenin global olarak benzersiz kimliğini alır. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Geçmişin etkinleştirilip etkinleştirilmediğini gösteren bir değer alır veya ayarlar. |
| [Item](../../aspose.note/notebook/item) { get; } | Verilen dizine göre not defteri alt düğümünü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Düğümü listenin sonuna ekler. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Tüm alt düğümleri düğüm türüne göre alın. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Alt düğümler arasında yinelenen bir Numaralandırıcı döndürür.[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | Bir alt belge düğümü ekler. Bir akıştan mevcut bir OneNote belgesini açar. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | Bir alt belge düğümü ekler. Bir dosyadan var olan bir OneNote belgesini açar. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | Bir alt belge düğümü ekler. Bir akıştan var olan bir OneNote belgesini açar. Ek yükleme seçeneklerini belirlemeye izin verir. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | Bir alt belge düğümü ekler. Bir dosyadan var olan bir OneNote belgesini açar. Ek yükleme seçeneklerini belirlemeye izin verir. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | Bir alt not defteri düğümü ekler. Bir akıştan mevcut bir OneNote not defterini açar. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | Bir alt not defteri düğümü ekler. Bir dosyadan mevcut bir OneNote not defterini açar. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Bir alt not defteri düğümü ekler. Bir akıştan mevcut bir OneNote not defterini açar. Ek yükleme seçeneklerini belirlemeye izin verir. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | Bir alt not defteri düğümü ekler. Bir dosyadan var olan bir OneNote not defterini açar. Ek yükleme seçeneklerini belirlemeye izin verir. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Alt düğümü kaldırır. |
| [Save](../../aspose.note/notebook/save#save)(Stream) | OneNote belgesini bir akışa kaydeder. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | OneNote belgesini bir dosyaya kaydeder. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak OneNote belgesini bir akışa kaydeder. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | OneNote belgesini belirtilen biçimde bir akışa kaydeder. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak OneNote belgesini bir dosyaya kaydeder. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | OneNote belgesini belirtilen biçimde bir dosyaya kaydeder. |

### Örnekler

Not defterinin nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Not Defterini Kaydet
notebook.Save(dataDir);
```

Not defterinin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Not Defterini Kaydet
notebook.Save(dataDir);
```

Not defterinin resim olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir);
```

Bir not defterinden tüm metnin nasıl alınacağını gösterir.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

Düzleştirilmiş not defterinin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Not Defterini Kaydet
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Onları tembelce yükleyen bir not defterinin belgeleri arasında nasıl yineleme yapılacağını gösterir.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Varsayılan olarak çocuk yüklemesi "tembel"dir.
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Alt belgenin fiili yüklemesi yalnızca burada gerçekleşir.
    // Alt belgeyle bir şeyler yap
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

Bir akıştan not defterinin nasıl yükleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Şifreli bir not defterinin nasıl yapıldığını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Belirtilen seçeneklerle not defterinin resim olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

Düzleştirilmiş not defterinin resim olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

Not defterinden bir bölümün nasıl kaldırılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote Not Defterini Yükle
var notebook = new Notebook(dataDir + "test.onetoc2");

// İstenen alt öğeyi aramak için alt düğümleri arasında gezin
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Alt Öğeyi Defterden Kaldır
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Not Defterini Kaydet
notebook.Save(dataDir);
```

Bir not defterinin önceden yüklenmiş belgeleri arasında nasıl yineleme yapılacağını gösterir.

```csharp
// Varsayılan olarak çocuk yüklemesi "tembel"dir.
// Bu nedenle anlık yükleme için gerçekleşmiş,
// NotebookLoadOptions.InstantLoading bayrağını ayarlamak gerekiyor.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Tüm alt belgeler zaten yüklendi.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Alt belgeyle bir şeyler yap
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

### Ayrıca bakınız

* interface [INotebookChildNode](../inotebookchildnode)
* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
