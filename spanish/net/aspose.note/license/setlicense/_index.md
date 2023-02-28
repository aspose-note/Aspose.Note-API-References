---
title: License.SetLicense
second_title: Aspose.Note para la referencia de la API de .NET
description: License método. Licencia el componente.
type: docs
weight: 20
url: /es/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licencia el componente.

```csharp
public void SetLicense(string licenseName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| licenseName | String | Puede ser un nombre de archivo completo o corto o el nombre de un recurso incrustado. Use una cadena vacía para cambiar al modo de evaluación. |

### Observaciones

Intenta encontrar la licencia en las siguientes ubicaciones:

1. Ruta explícita.

2. La carpeta que contiene el ensamblaje del componente Aspose.

3. La carpeta que contiene el ensamblado de llamada del cliente.

4. La carpeta que contiene el ensamblado de entrada (inicio).

5. Un recurso incrustado en el ensamblado de llamadas del cliente.

**Nota:**En .NET Compact Framework, intenta encontrar la licencia solo en estas ubicaciones:

1. Ruta explícita.

2. Un recurso incrustado en el ensamblado de llamadas del cliente.

### Ejemplos

Muestra cómo cargar una licencia para Aspose.Note desde un archivo.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Muestra cómo cargar una licencia para Aspose.Note desde un recurso de archivo incrustado.

```csharp
// Instanciar la clase de Licencia
Aspose.Note.License license = new Aspose.Note.License();

// Pasar solo el nombre del archivo de licencia incrustado en el ensamblado
license.SetLicense("Aspose.Note.lic");
```

### Ver también

* class [License](../)
* espacio de nombres [Aspose.Note](../../license/)
* asamblea [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Licencia el componente.

```csharp
public void SetLicense(Stream stream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | Un flujo que contiene la licencia. |

### Observaciones

Utilice este método para cargar una licencia desde una transmisión.

### Ejemplos

Muestra cómo cargar una licencia para Aspose.Note desde una secuencia.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Ver también

* class [License](../)
* espacio de nombres [Aspose.Note](../../license/)
* asamblea [Aspose.Note](../../../)


