---
title: Document
second_title: Aspose.Note för .NET API-referens
description: Initierar en ny instans avDocumentaspose.note/document class. Skapar ett tomt OneNote-dokument.
type: docs
weight: 10
url: /sv/net/aspose.note/document/document/
---
## Document() {#constructor}

Initierar en ny instans av[`Document`](../../document) class. Skapar ett tomt OneNote-dokument.

```csharp
public Document()
```

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Initierar en ny instans av[`Document`](../../document) class. Öppnar ett befintligt OneNote-dokument från en fil.

```csharp
public Document(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |

### Undantag

| undantag | skick |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Dokumentformatet känns inte igen eller stöds inte. |
| [FileCorruptedException](../../filecorruptedexception) | Dokumentet verkar vara skadat och kan inte laddas. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Dokumentet är krypterat och kräver ett lösenord för att öppnas, men du har angett ett felaktigt lösenord. |
| InvalidOperationException | Det finns ett problem med dokumentet och det bör rapporteras till Aspose.Note-utvecklare. |
| IOException | Det finns ett input/output undantag. |

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Initierar en ny instans av[`Document`](../../document) class. Öppnar ett befintligt OneNote-dokument från en fil. Tillåter att ange ytterligare alternativ såsom ett krypteringslösenord.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |
| loadOptions | LoadOptions | Alternativ som används för att ladda ett dokument. Kan vara null. |

### Undantag

| undantag | skick |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Dokumentformatet känns inte igen eller stöds inte. |
| [FileCorruptedException](../../filecorruptedexception) | Dokumentet verkar vara skadat och kan inte laddas. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Dokumentet är krypterat och kräver ett lösenord för att öppnas, men du har angett ett felaktigt lösenord. |
| InvalidOperationException | Det finns ett problem med dokumentet och det bör rapporteras till Aspose.Note-utvecklare. |
| IOException | Det finns ett input/output undantag. |

### Se även

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Initierar en ny instans av[`Document`](../../document) class. Öppnar ett befintligt OneNote-dokument från en ström.

```csharp
public Document(Stream inStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inStream | Stream | Strömmen. |

### Undantag

| undantag | skick |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Dokumentformatet känns inte igen eller stöds inte. |
| [FileCorruptedException](../../filecorruptedexception) | Dokumentet verkar vara skadat och kan inte laddas. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Dokumentet är krypterat och kräver ett lösenord för att öppnas, men du har angett ett felaktigt lösenord. |
| InvalidOperationException | Det finns ett problem med dokumentet och det bör rapporteras till Aspose.Note-utvecklare. |
| IOException | Det finns ett input/output undantag. |
| ArgumentException | Strömmen stöder inte läsning, är null eller är redan stängd. |

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Initierar en ny instans av[`Document`](../../document) class. Öppnar ett befintligt OneNote-dokument från en ström. Tillåter att ange ytterligare alternativ såsom ett krypteringslösenord.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inStream | Stream | Strömmen. |
| loadOptions | LoadOptions | Alternativ som används för att ladda ett dokument. Kan vara null. |

### Undantag

| undantag | skick |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Dokumentformatet känns inte igen eller stöds inte. |
| [FileCorruptedException](../../filecorruptedexception) | Dokumentet verkar vara skadat och kan inte laddas. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Dokumentet är krypterat och kräver ett lösenord för att öppnas, men du har angett ett felaktigt lösenord. |
| InvalidOperationException | Det finns ett problem med dokumentet och det bör rapporteras till Aspose.Note-utvecklare. |
| IOException | Det finns ett input/output undantag. |
| ArgumentException | Strömmen stöder inte läsning, är null eller är redan stängd. |

### Se även

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
