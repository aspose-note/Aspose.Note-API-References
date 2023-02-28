---
title: Class NotebookLoadOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.NotebookLoadOptions sınıf. Not defteri yüklemek için kullanılan seçenekler.
type: docs
weight: 420
url: /tr/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Not defteri yüklemek için kullanılan seçenekler.

```csharp
public class NotebookLoadOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Alt belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değer alır veya ayarlar. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Üst belge yüklenirken alt belgelerin yüklenmesi gerekip gerekmediğini belirten bir değer alır veya ayarlar. |

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

* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


