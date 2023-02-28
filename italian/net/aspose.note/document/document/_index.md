---
title: Document.Document
second_title: Aspose.Note per .NET API Reference
description: Document costruttore. Inizializza una nuova istanza diDocument class. Crea un documento OneNote vuoto.
type: docs
weight: 10
url: /it/net/aspose.note/document/document/
---
## Document() {#constructor}

Inizializza una nuova istanza di[`Document`](../) class. Crea un documento OneNote vuoto.

```csharp
public Document()
```

### Guarda anche

* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Inizializza una nuova istanza di[`Document`](../) class. Apre un documento OneNote esistente da un file.

```csharp
public Document(string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Il formato del documento non è riconosciuto o non è supportato. |
| [FileCorruptedException](../../filecorruptedexception/) | Il documento sembra danneggiato e non può essere caricato. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Il documento è crittografato e richiede una password per essere aperto, ma hai fornito una password errata. |
| InvalidOperationException | C'è un problema con il documento e dovrebbe essere segnalato agli sviluppatori di Aspose.Note. |
| IOException | È presente un'eccezione di input/output. |

### Guarda anche

* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Inizializza una nuova istanza di[`Document`](../)class. Apre un documento OneNote esistente da un file. Consente di specificare opzioni aggiuntive come una password di crittografia.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| loadOptions | LoadOptions | Opzioni utilizzate per caricare un documento. Può essere nullo. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Il formato del documento non è riconosciuto o non è supportato. |
| [FileCorruptedException](../../filecorruptedexception/) | Il documento sembra danneggiato e non può essere caricato. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Il documento è crittografato e richiede una password per essere aperto, ma hai fornito una password errata. |
| InvalidOperationException | C'è un problema con il documento e dovrebbe essere segnalato agli sviluppatori di Aspose.Note. |
| IOException | È presente un'eccezione di input/output. |

### Guarda anche

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Inizializza una nuova istanza di[`Document`](../) class. Apre un documento OneNote esistente da uno stream.

```csharp
public Document(Stream inStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inStream | Stream | Il flusso. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Il formato del documento non è riconosciuto o non è supportato. |
| [FileCorruptedException](../../filecorruptedexception/) | Il documento sembra danneggiato e non può essere caricato. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Il documento è crittografato e richiede una password per essere aperto, ma hai fornito una password errata. |
| InvalidOperationException | C'è un problema con il documento e dovrebbe essere segnalato agli sviluppatori di Aspose.Note. |
| IOException | È presente un'eccezione di input/output. |
| ArgumentException | Il flusso non supporta la lettura, è nullo o è già chiuso. |

### Guarda anche

* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Inizializza una nuova istanza di[`Document`](../) class. Apre un documento OneNote esistente da un flusso. Consente di specificare opzioni aggiuntive come una password di crittografia.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inStream | Stream | Il flusso. |
| loadOptions | LoadOptions | Opzioni utilizzate per caricare un documento. Può essere nullo. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Il formato del documento non è riconosciuto o non è supportato. |
| [FileCorruptedException](../../filecorruptedexception/) | Il documento sembra danneggiato e non può essere caricato. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Il documento è crittografato e richiede una password per essere aperto, ma hai fornito una password errata. |
| InvalidOperationException | C'è un problema con il documento e dovrebbe essere segnalato agli sviluppatori di Aspose.Note. |
| IOException | È presente un'eccezione di input/output. |
| ArgumentException | Il flusso non supporta la lettura, è nullo o è già chiuso. |

### Guarda anche

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)


