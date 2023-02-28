---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note per .NET API Reference
description: ImageBinarizationOptions proprietà. Ottiene o imposta il valore di soglia per il metodo di binarizzazione a soglia fissa. Il valore predefinito è 128.
type: docs
weight: 30
url: /it/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Ottiene o imposta il valore di soglia per il metodo di binarizzazione a soglia fissa. Il valore predefinito è 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Esempi

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

* class [ImageBinarizationOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../imagebinarizationoptions/)
* assemblea [Aspose.Note](../../../)


