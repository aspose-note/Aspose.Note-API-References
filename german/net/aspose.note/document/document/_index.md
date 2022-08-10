---
title: Document
second_title: Aspose.Note für .NET-API-Referenz
description: Initialisiert eine neue Instanz vonDocumentaspose.note/document class. Erstellt ein leeres OneNote-Dokument.
type: docs
weight: 10
url: /de/net/aspose.note/document/document/
---
## Document() {#constructor}

Initialisiert eine neue Instanz von[`Document`](../../document) class. Erstellt ein leeres OneNote-Dokument.

```csharp
public Document()
```

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Initialisiert eine neue Instanz von[`Document`](../../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei.

```csharp
public Document(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Das Dokumentformat wird nicht erkannt oder nicht unterstützt. |
| [FileCorruptedException](../../filecorruptedexception) | Das Dokument scheint beschädigt zu sein und kann nicht geladen werden. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Das Dokument ist verschlüsselt und zum Öffnen ist ein Kennwort erforderlich, aber Sie haben ein falsches Kennwort angegeben. |
| InvalidOperationException | Es liegt ein Problem mit dem Dokument vor, das den Aspose.Note-Entwicklern gemeldet werden sollte. |
| IOException | Es liegt eine Ein-/Ausgabeausnahme vor. |

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Initialisiert eine neue Instanz von[`Document`](../../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. Ermöglicht die Angabe zusätzlicher Optionen wie z. B. eines Verschlüsselungskennworts.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |
| loadOptions | LoadOptions | Optionen zum Laden eines Dokuments. Kann null sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Das Dokumentformat wird nicht erkannt oder nicht unterstützt. |
| [FileCorruptedException](../../filecorruptedexception) | Das Dokument scheint beschädigt zu sein und kann nicht geladen werden. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Das Dokument ist verschlüsselt und zum Öffnen ist ein Kennwort erforderlich, aber Sie haben ein falsches Kennwort angegeben. |
| InvalidOperationException | Es liegt ein Problem mit dem Dokument vor, das den Aspose.Note-Entwicklern gemeldet werden sollte. |
| IOException | Es liegt eine Ein-/Ausgabeausnahme vor. |

### Siehe auch

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`Document`](../../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream.

```csharp
public Document(Stream inStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inStream | Stream | Der Strom. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Das Dokumentformat wird nicht erkannt oder nicht unterstützt. |
| [FileCorruptedException](../../filecorruptedexception) | Das Dokument scheint beschädigt zu sein und kann nicht geladen werden. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Das Dokument ist verschlüsselt und zum Öffnen ist ein Kennwort erforderlich, aber Sie haben ein falsches Kennwort angegeben. |
| InvalidOperationException | Es liegt ein Problem mit dem Dokument vor, das den Aspose.Note-Entwicklern gemeldet werden sollte. |
| IOException | Es liegt eine Ein-/Ausgabeausnahme vor. |
| ArgumentException | Der Stream unterstützt kein Lesen, ist null oder bereits geschlossen. |

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Initialisiert eine neue Instanz von[`Document`](../../document) class. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. Ermöglicht die Angabe zusätzlicher Optionen wie z. B. eines Verschlüsselungskennworts.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inStream | Stream | Der Strom. |
| loadOptions | LoadOptions | Optionen zum Laden eines Dokuments. Kann null sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Das Dokumentformat wird nicht erkannt oder nicht unterstützt. |
| [FileCorruptedException](../../filecorruptedexception) | Das Dokument scheint beschädigt zu sein und kann nicht geladen werden. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Das Dokument ist verschlüsselt und zum Öffnen ist ein Kennwort erforderlich, aber Sie haben ein falsches Kennwort angegeben. |
| InvalidOperationException | Es liegt ein Problem mit dem Dokument vor, das den Aspose.Note-Entwicklern gemeldet werden sollte. |
| IOException | Es liegt eine Ein-/Ausgabeausnahme vor. |
| ArgumentException | Der Stream unterstützt kein Lesen, ist null oder bereits geschlossen. |

### Siehe auch

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
