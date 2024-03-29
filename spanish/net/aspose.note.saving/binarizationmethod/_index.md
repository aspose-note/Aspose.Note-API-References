---
title: Enum BinarizationMethod
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Saving.BinarizationMethod enumeración. Especifica el método de binarización para una imagen.
type: docs
weight: 560
url: /es/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Especifica el método de binarización para una imagen.

```csharp
public enum BinarizationMethod
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FixedThreshold | `0` | La binarización de la imagen se realiza utilizando el umbral fijo especificado. |
| Otsu | `1` | La binarización de la imagen se realiza de forma adaptativa utilizando el método de Otsu para evaluar el umbral. |

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

* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving/)
* asamblea [Aspose.Note](../../)


