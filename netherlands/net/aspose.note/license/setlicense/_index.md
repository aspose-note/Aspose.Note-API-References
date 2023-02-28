---
title: License.SetLicense
second_title: Aspose.Note voor .NET API-referentie
description: License methode. Licentie voor de component.
type: docs
weight: 20
url: /nl/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licentie voor de component.

```csharp
public void SetLicense(string licenseName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| licenseName | String | Kan een volledige of korte bestandsnaam zijn of de naam van een ingebedde bron. Gebruik een lege tekenreeks om over te schakelen naar de evaluatiemodus. |

### Opmerkingen

Probeert de licentie te vinden op de volgende locaties:

1. Expliciet pad.

2. De map die de Aspose component-assembly bevat.

3. De map die de aanroepende assembly van de client bevat.

4. De map die de entry (opstart)-assembly bevat.

5. Een ingesloten bron in de aanroepende assembly van de client.

**Opmerking:**Probeert op het .NET Compact Framework de licentie alleen op deze locaties te vinden:

1. Expliciet pad.

2. Een ingesloten bron in de aanroepende assembly van de client.

### Voorbeelden

Laat zien hoe u een licentie voor Aspose.Note laadt vanuit een bestand.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Laat zien hoe u een licentie voor Aspose.Note kunt laden vanuit een ingesloten bestandsbron.

```csharp
// Instantiseer de License-klasse
Aspose.Note.License license = new Aspose.Note.License();

// Geef alleen de naam door van het licentiebestand dat in de assembly is ingesloten
license.SetLicense("Aspose.Note.lic");
```

### Zie ook

* class [License](../)
* naamruimte [Aspose.Note](../../license/)
* montage [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Licentie voor de component.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | Een stream die de licentie bevat. |

### Opmerkingen

Gebruik deze methode om een licentie van een stream te laden.

### Voorbeelden

Laat zien hoe u een licentie voor Aspose.Note laadt vanuit een stream.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Zie ook

* class [License](../)
* naamruimte [Aspose.Note](../../license/)
* montage [Aspose.Note](../../../)


