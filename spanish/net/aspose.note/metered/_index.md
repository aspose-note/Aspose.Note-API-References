---
title: Class Metered
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Metered clase. Proporciona métodos para configurar la clave medida.
type: docs
weight: 350
url: /es/net/aspose.note/metered/
---
## Metered class

Proporciona métodos para configurar la clave medida.

```csharp
public class Metered
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Metered](metered/)() | Constructor predeterminado |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Elimina la licencia de instalación anterior. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Establece claves públicas y privadas medidas. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Obtiene crédito de consumo. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Obtiene el tamaño del archivo de consumo. |

### Ejemplos

En este ejemplo, se intentará establecer una clave pública y privada medidas

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

Muestra cómo configurar la licencia medida.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Ver también

* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


