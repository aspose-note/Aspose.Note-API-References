---
title: Class License
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.License klas. Biedt methoden om de component te licentiëren.
type: docs
weight: 310
url: /nl/net/aspose.note/license/
---
## License class

Biedt methoden om de component te licentiëren.

```csharp
public class License
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [License](license/)() | De standaard constructeur. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Licentie voor de component. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Licentie voor de component. |

### Voorbeelden

Laat zien hoe u een licentie voor Aspose.Note laadt vanuit een bestand.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Laat zien hoe u een licentie voor Aspose.Note laadt vanuit een stream.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Laat zien hoe u een licentie voor Aspose.Note kunt laden vanuit een ingesloten bestandsbron.

```csharp
// Instantiseer de License-klasse
Aspose.Note.License license = new Aspose.Note.License();

// Geef alleen de naam door van het licentiebestand dat in de assembly is ingesloten
license.SetLicense("Aspose.Note.lic");
```

### Zie ook

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


