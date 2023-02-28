---
title: ImageBinarizationOptions.BinarizationMethod
second_title: Aspose.Note per .NET API Reference
description: ImageBinarizationOptions proprietà. Ottiene o imposta il metodo di binarizzazione. Il valore predefinito èFixedThreshold .
type: docs
weight: 20
url: /it/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

Ottiene o imposta il metodo di binarizzazione. Il valore predefinito èFixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

### Esempi

Mostra come salvare un documento come immagine binaria usando il metodo di Otsu.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Salva il documento come gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Mostra come salvare un documento come immagine binaria utilizzando una soglia fissa.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Salva il documento come gif.
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

### Guarda anche

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../imagebinarizationoptions/)
* assemblea [Aspose.Note](../../../)


