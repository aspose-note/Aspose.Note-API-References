---
title: Class License
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.License clase. Proporciona métodos para licenciar el componente.
type: docs
weight: 310
url: /es/net/aspose.note/license/
---
## License class

Proporciona métodos para licenciar el componente.

```csharp
public class License
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [License](license/)() | Constructor predeterminado |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Licencia el componente. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Licencia el componente. |

### Ejemplos

Muestra cómo cargar una licencia para Aspose.Note desde un archivo.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Muestra cómo cargar una licencia para Aspose.Note desde una secuencia.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Muestra cómo cargar una licencia para Aspose.Note desde un recurso de archivo incrustado.

```csharp
// Instanciar la clase de Licencia
Aspose.Note.License license = new Aspose.Note.License();

// Pasar solo el nombre del archivo de licencia incrustado en el ensamblado
license.SetLicense("Aspose.Note.lic");
```

### Ver también

* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


