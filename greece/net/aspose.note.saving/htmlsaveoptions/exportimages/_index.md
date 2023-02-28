---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note for .NET API Reference
description: HtmlSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων.
type: docs
weight: 70
url: /el/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων.

```csharp
public ResourceExportType ExportImages { get; set; }
```

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή html με την αποθήκευση όλων των πόρων (css/fonts/εικόνες) σε ξεχωριστά αρχεία.

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

Δείχνει τον τρόπο αποθήκευσης ενός εγγράφου σε ροή σε μορφή html με ενσωμάτωση όλων των πόρων (css/fonts/images).

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

### Δείτε επίσης

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../htmlsaveoptions/)
* συνέλευση [Aspose.Note](../../../)


