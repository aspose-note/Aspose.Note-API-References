---
title: ImageSaveOptions.BinarizationOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: ImageSaveOptions propiedad. Obtiene o establece opciones para la binarización de la imagen.
type: docs
weight: 20
url: /es/net/aspose.note.saving/imagesaveoptions/binarizationoptions/
---
## ImageSaveOptions.BinarizationOptions property

Obtiene o establece opciones para la binarización de la imagen.

```csharp
public ImageBinarizationOptions BinarizationOptions { get; set; }
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

* class [ImageBinarizationOptions](../../imagebinarizationoptions/)
* class [ImageSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../imagesaveoptions/)
* asamblea [Aspose.Note](../../../)


