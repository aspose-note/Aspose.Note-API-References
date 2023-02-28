---
title: ImageSaveOptions.BinarizationOptions
second_title: Aspose.Note für .NET-API-Referenz
description: ImageSaveOptions eigendom. Ruft Optionen für die Binarisierung von Bildern ab oder legt sie fest.
type: docs
weight: 20
url: /de/net/aspose.note.saving/imagesaveoptions/binarizationoptions/
---
## ImageSaveOptions.BinarizationOptions property

Ruft Optionen für die Binarisierung von Bildern ab oder legt sie fest.

```csharp
public ImageBinarizationOptions BinarizationOptions { get; set; }
```

### Beispiele

Zeigt, wie ein Dokument mit der Methode von Otsu als Binärbild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Speichern Sie das Dokument als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Zeigt, wie ein Dokument als Binärbild mit festem Schwellenwert gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Speichern Sie das Dokument als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### Siehe auch

* class [ImageBinarizationOptions](../../imagebinarizationoptions/)
* class [ImageSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../imagesaveoptions/)
* Montage [Aspose.Note](../../../)


