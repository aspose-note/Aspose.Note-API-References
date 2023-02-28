---
title: Class License
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.License klas. Stellt Methoden zur Lizenzierung der Komponente bereit.
type: docs
weight: 310
url: /de/net/aspose.note/license/
---
## License class

Stellt Methoden zur Lizenzierung der Komponente bereit.

```csharp
public class License
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [License](license/)() | Default_Constructor |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Lizenziert die Komponente. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Lizenziert die Komponente. |

### Beispiele

Zeigt, wie eine Lizenz für Aspose.Note aus einer Datei geladen wird.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Zeigt, wie eine Lizenz für Aspose.Note aus einem Stream geladen wird.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Zeigt, wie eine Lizenz für Aspose.Note aus einer eingebetteten Dateiressource geladen wird.

```csharp
// Lizenzklasse instanziieren
Aspose.Note.License license = new Aspose.Note.License();

// Übergeben Sie nur den Namen der in die Assembly eingebetteten Lizenzdatei
license.SetLicense("Aspose.Note.lic");
```

### Siehe auch

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


