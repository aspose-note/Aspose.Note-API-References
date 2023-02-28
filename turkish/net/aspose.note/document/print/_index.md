---
title: Document.Print
second_title: Aspose.Note for .NET API Referansı
description: Document yöntem. Varsayılan yazıcıyı kullanarak belgeyi yazdırır.
type: docs
weight: 130
url: /tr/net/aspose.note/document/print/
---
## Print() {#print}

Varsayılan yazıcıyı kullanarak belgeyi yazdırır.

```csharp
public void Print()
```

### Örnekler

Varsayılan seçeneklerle standart Windows iletişim kutusunu kullanarak belgenin bir yazıcıya nasıl gönderileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### Ayrıca bakınız

* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Varsayılan yazıcıyı kullanarak belgeyi yazdırır.

```csharp
public void Print(PrintOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | PrintOptions | Bir belgeyi yazdırmak için kullanılan seçenekler. Boş olabilir. |

### Ayrıca bakınız

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


