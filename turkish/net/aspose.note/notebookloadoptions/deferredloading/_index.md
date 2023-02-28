---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note for .NET API Referansı
description: NotebookLoadOptions mülk. Alt belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değer alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Alt belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değer alır veya ayarlar.

```csharp
public bool DeferredLoading { get; set; }
```

### Notlar

Varsayılan değer:`YANLIŞ` , böylece alt belgeler dolaylı olarak yüklenecektir. Değer`doğru` kullanıcının araması gerektiğini gösteriyor[`LoadChildDocument`](../../notebook/loadchilddocument/) veya not defterinin kendisi yüklendikten sonra her not defterinin alt düğümü için. Değer ise`doğru` ,[`InstantLoading`](../instantloading/) seçenek yoksayılacak. Not defteri akıştan yükleniyorsa, değer her zaman`doğru` kullanıcı tarafından açıkça ayarlanmış olmasına rağmen`YANLIŞ` .

### Örnekler

Not defterinin nasıl şifreleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Ayrıca bakınız

* class [NotebookLoadOptions](../)
* ad alanı [Aspose.Note](../../notebookloadoptions/)
* toplantı [Aspose.Note](../../../)


