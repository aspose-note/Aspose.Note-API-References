---
title: CheckBox.SetCompleted
second_title: Aspose.Note per .NET API Reference
description: CheckBox metodo. Imposta il tag sullo stato completato.
type: docs
weight: 70
url: /it/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Imposta il tag sullo stato completato.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| completedTime | DateTime | Il tempo completato. |

### Guarda anche

* class [CheckBox](../)
* spazio dei nomi [Aspose.Note](../../checkbox/)
* assemblea [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Imposta il tag sullo stato completato utilizzando l'ora corrente come ora completata.

```csharp
public void SetCompleted()
```

### Esempi

Mostra come completare tutti gli elementi della casella di controllo relativi al "Progetto C".

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

### Guarda anche

* class [CheckBox](../)
* spazio dei nomi [Aspose.Note](../../checkbox/)
* assemblea [Aspose.Note](../../../)


