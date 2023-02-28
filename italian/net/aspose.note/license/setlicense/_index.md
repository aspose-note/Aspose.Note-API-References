---
title: License.SetLicense
second_title: Aspose.Note per .NET API Reference
description: License metodo. Concede in licenza il componente.
type: docs
weight: 20
url: /it/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Concede in licenza il componente.

```csharp
public void SetLicense(string licenseName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| licenseName | String | Può essere un nome file completo o breve o il nome di una risorsa incorporata. Usa una stringa vuota per passare alla modalità di valutazione. |

### Osservazioni

Tenta di trovare la licenza nelle seguenti posizioni:

1. Percorso esplicito.

2. La cartella che contiene l'assieme del componente Aspose.

3. La cartella che contiene l'assembly chiamante del client.

4. La cartella che contiene l'assembly della voce (avvio).

5. Una risorsa incorporata nell'assembly chiamante del client.

**Nota:**In .NET Compact Framework, tenta di trovare la licenza solo in questi percorsi:

1. Percorso esplicito.

2. Una risorsa incorporata nell'assembly chiamante del client.

### Esempi

Mostra come caricare una licenza per Aspose.Note da un file.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Mostra come caricare una licenza per Aspose.Note dalla risorsa file incorporata.

```csharp
// Crea un'istanza della classe License
Aspose.Note.License license = new Aspose.Note.License();

// Passa solo il nome del file di licenza incorporato nell'assembly
license.SetLicense("Aspose.Note.lic");
```

### Guarda anche

* class [License](../)
* spazio dei nomi [Aspose.Note](../../license/)
* assemblea [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Concede in licenza il componente.

```csharp
public void SetLicense(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Un flusso che contiene la licenza. |

### Osservazioni

Utilizzare questo metodo per caricare una licenza da un flusso.

### Esempi

Mostra come caricare una licenza per Aspose.Note da un flusso.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Guarda anche

* class [License](../)
* spazio dei nomi [Aspose.Note](../../license/)
* assemblea [Aspose.Note](../../../)


