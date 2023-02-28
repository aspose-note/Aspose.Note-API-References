---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note für .NET-API-Referenz
description: ImageBinarizationOptions eigendom. Ruft den Schwellenwert für die Binarisierungsmethode mit festem Schwellenwert ab oder legt ihn fest. Der Standardwert ist 128.
type: docs
weight: 30
url: /de/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Ruft den Schwellenwert für die Binarisierungsmethode mit festem Schwellenwert ab oder legt ihn fest. Der Standardwert ist 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Beispiele

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

* class [ImageBinarizationOptions](../)
* namensraum [Aspose.Note.Saving](../../imagebinarizationoptions/)
* Montage [Aspose.Note](../../../)


