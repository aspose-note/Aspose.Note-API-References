---
title: ImageBinarizationOptions.BinarizationMethod
second_title: Aspose.Note para la referencia de la API de .NET
description: ImageBinarizationOptions propiedad. Obtiene o establece el método de binarización. El valor predeterminado esFixedThreshold .
type: docs
weight: 20
url: /es/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

Obtiene o establece el método de binarización. El valor predeterminado esFixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

### Ejemplos

Muestra cómo guardar un documento como imagen binaria usando el método de Otsu.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Guarda el documento como gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Muestra cómo guardar un documento como imagen binaria utilizando un umbral fijo.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Guarda el documento como gif.
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

### Ver también

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../imagebinarizationoptions/)
* asamblea [Aspose.Note](../../../)


