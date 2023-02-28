---
title: Class License
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.License classe. Fornisce metodi per concedere in licenza il componente.
type: docs
weight: 310
url: /it/net/aspose.note/license/
---
## License class

Fornisce metodi per concedere in licenza il componente.

```csharp
public class License
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [License](license/)() | Default_Costruttore |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Concede in licenza il componente. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Concede in licenza il componente. |

### Esempi

Mostra come caricare una licenza per Aspose.Note da un file.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Mostra come caricare una licenza per Aspose.Note da un flusso.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Mostra come caricare una licenza per Aspose.Note dalla risorsa file incorporata.

```csharp
// Crea un'istanza della classe License
Aspose.Note.License license = new Aspose.Note.License();

// Passa solo il nome del file di licenza incorporato nell'assembly
license.SetLicense("Aspose.Note.lic");
```

### Guarda anche

* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


