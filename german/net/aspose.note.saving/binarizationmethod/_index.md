---
title: Enum BinarizationMethod
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.BinarizationMethod opsomming. Gibt die Binärisierungsmethode für ein Bild an.
type: docs
weight: 560
url: /de/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Gibt die Binärisierungsmethode für ein Bild an.

```csharp
public enum BinarizationMethod
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| FixedThreshold | `0` | Die Binarisierung des Bildes wird mit einem festgelegten festen Schwellenwert durchgeführt. |
| Otsu | `1` | Die Binarisierung des Bildes erfolgt adaptiv unter Verwendung der Methode von Otsu zur Bewertung des Schwellenwerts. |

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

* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


