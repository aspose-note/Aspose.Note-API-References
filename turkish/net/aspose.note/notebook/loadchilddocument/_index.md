---
title: Notebook.LoadChildDocument
second_title: Aspose.Note for .NET API Referansı
description: Notebook yöntem. Bir alt belge düğümü ekler. Bir dosyadan mevcut bir OneNote belgesini açar.
type: docs
weight: 120
url: /tr/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

Bir alt belge düğümü ekler. Bir dosyadan mevcut bir OneNote belgesini açar.

```csharp
public void LoadChildDocument(string filePath)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |

### Örnekler

Not defterinin bir akıştan nasıl yükleneceğini gösterir.

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

### Ayrıca bakınız

* class [Notebook](../)
* ad alanı [Aspose.Note](../../notebook/)
* toplantı [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

Bir alt belge düğümü ekler. Mevcut bir OneNote belgesini bir dosyadan açar. Ek yükleme seçeneklerini belirlemeye izin verir.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| loadOptions | LoadOptions | Yükleme seçenekleri. |

### Ayrıca bakınız

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* ad alanı [Aspose.Note](../../notebook/)
* toplantı [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

Bir alt belge düğümü ekler. Bir akıştan mevcut bir OneNote belgesini açar.

```csharp
public void LoadChildDocument(Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Akış. |

### Örnekler

Not defterinin bir akıştan nasıl yükleneceğini gösterir.

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

### Ayrıca bakınız

* class [Notebook](../)
* ad alanı [Aspose.Note](../../notebook/)
* toplantı [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

Bir alt belge düğümü ekler. Bir akıştan mevcut bir OneNote belgesini açar. Ek yükleme seçeneklerini belirlemeye izin verir.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Akış. |
| loadOptions | LoadOptions | Yükleme seçenekleri. |

### Ayrıca bakınız

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* ad alanı [Aspose.Note](../../notebook/)
* toplantı [Aspose.Note](../../../)


