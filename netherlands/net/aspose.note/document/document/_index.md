---
title: Document.Document
second_title: Aspose.Note voor .NET API-referentie
description: Document constructeur. Initialiseert een nieuw exemplaar van hetDocument class. Maakt een leeg OneNotedocument aan.
type: docs
weight: 10
url: /nl/net/aspose.note/document/document/
---
## Document() {#constructor}

Initialiseert een nieuw exemplaar van het[`Document`](../) class. Maakt een leeg OneNote-document aan.

```csharp
public Document()
```

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Initialiseert een nieuw exemplaar van het[`Document`](../) class. Opent een bestaand OneNote-document vanuit een bestand.

```csharp
public Document(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Het documentformaat wordt niet herkend of niet ondersteund. |
| [FileCorruptedException](../../filecorruptedexception/) | Het document lijkt beschadigd te zijn en kan niet worden geladen. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Het document is gecodeerd en vereist een wachtwoord om te openen, maar u heeft een onjuist wachtwoord opgegeven. |
| InvalidOperationException | Er is een probleem met het document en dit moet worden gemeld aan de ontwikkelaars van Aspose.Note. |
| IOException | Er is een invoer/uitvoer-uitzondering. |

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Initialiseert een nieuw exemplaar van het[`Document`](../)class. Opent een bestaand OneNote-document vanuit een bestand. Maakt het mogelijk om extra opties op te geven, zoals een coderingswachtwoord.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |
| loadOptions | LoadOptions | Opties die worden gebruikt om een document te laden. Kan nul zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Het documentformaat wordt niet herkend of niet ondersteund. |
| [FileCorruptedException](../../filecorruptedexception/) | Het document lijkt beschadigd te zijn en kan niet worden geladen. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Het document is gecodeerd en vereist een wachtwoord om te openen, maar u heeft een onjuist wachtwoord opgegeven. |
| InvalidOperationException | Er is een probleem met het document en dit moet worden gemeld aan de ontwikkelaars van Aspose.Note. |
| IOException | Er is een invoer/uitvoer-uitzondering. |

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Document`](../) class. Opent een bestaand OneNote-document uit een stream.

```csharp
public Document(Stream inStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inStream | Stream | De stroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Het documentformaat wordt niet herkend of niet ondersteund. |
| [FileCorruptedException](../../filecorruptedexception/) | Het document lijkt beschadigd te zijn en kan niet worden geladen. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Het document is gecodeerd en vereist een wachtwoord om te openen, maar u heeft een onjuist wachtwoord opgegeven. |
| InvalidOperationException | Er is een probleem met het document en dit moet worden gemeld aan de ontwikkelaars van Aspose.Note. |
| IOException | Er is een invoer/uitvoer-uitzondering. |
| ArgumentException | De stream ondersteunt lezen niet, is null of is al gesloten. |

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`Document`](../) class. Opent een bestaand OneNote-document vanuit een stream. Maakt het mogelijk om extra opties op te geven, zoals een coderingswachtwoord.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inStream | Stream | De stroom. |
| loadOptions | LoadOptions | Opties die worden gebruikt om een document te laden. Kan nul zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Het documentformaat wordt niet herkend of niet ondersteund. |
| [FileCorruptedException](../../filecorruptedexception/) | Het document lijkt beschadigd te zijn en kan niet worden geladen. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Het document is gecodeerd en vereist een wachtwoord om te openen, maar u heeft een onjuist wachtwoord opgegeven. |
| InvalidOperationException | Er is een probleem met het document en dit moet worden gemeld aan de ontwikkelaars van Aspose.Note. |
| IOException | Er is een invoer/uitvoer-uitzondering. |
| ArgumentException | De stream ondersteunt lezen niet, is null of is al gesloten. |

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


