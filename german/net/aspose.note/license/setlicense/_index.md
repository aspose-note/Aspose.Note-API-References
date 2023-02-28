---
title: License.SetLicense
second_title: Aspose.Note für .NET-API-Referenz
description: License methode. Lizenziert die Komponente.
type: docs
weight: 20
url: /de/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Lizenziert die Komponente.

```csharp
public void SetLicense(string licenseName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| licenseName | String | Kann ein vollständiger oder kurzer Dateiname oder Name einer eingebetteten Ressource sein. Verwenden Sie eine leere Zeichenfolge, um in den Evaluierungsmodus zu wechseln. |

### Bemerkungen

Versucht, die Lizenz an den folgenden Orten zu finden:

1. Explizite Pfad.

2. Der Ordner, der die Aspose-Komponentenbaugruppe enthält.

3. Der Ordner, der die aufrufende Assembly des Clients enthält.

4. Der Ordner, der den Eintrag (Startup) Assembly enthält.

5. Eine eingebettete Ressource in der aufrufenden Assembly des Clients.

**Notiz:**Versucht in .NET Compact Framework, die Lizenz nur an diesen Speicherorten zu finden:

1. Explizite Pfad.

2. Eine eingebettete Ressource in der aufrufenden Assembly des Clients.

### Beispiele

Zeigt, wie eine Lizenz für Aspose.Note aus einer Datei geladen wird.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Zeigt, wie eine Lizenz für Aspose.Note aus einer eingebetteten Dateiressource geladen wird.

```csharp
// Lizenzklasse instanziieren
Aspose.Note.License license = new Aspose.Note.License();

// Übergeben Sie nur den Namen der in die Assembly eingebetteten Lizenzdatei
license.SetLicense("Aspose.Note.lic");
```

### Siehe auch

* class [License](../)
* namensraum [Aspose.Note](../../license/)
* Montage [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Lizenziert die Komponente.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Ein Stream, der die Lizenz enthält. |

### Bemerkungen

Verwenden Sie diese Methode, um eine Lizenz aus einem Stream zu laden.

### Beispiele

Zeigt, wie eine Lizenz für Aspose.Note aus einem Stream geladen wird.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Siehe auch

* class [License](../)
* namensraum [Aspose.Note](../../license/)
* Montage [Aspose.Note](../../../)


