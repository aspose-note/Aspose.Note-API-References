---
title: RichText.LastModifiedTime
second_title: Aspose.Note para la referencia de la API de .NET
description: RichText propiedad. Obtiene o establece la hora de última modificación.
type: docs
weight: 30
url: /es/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Obtiene o establece la hora de última modificación.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Ejemplos

Resaltemos los últimos cambios del texto resaltando.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Obtenga los nodos RichText modificados la semana pasada.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Establecer color de resaltado
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Establecer color de resaltado
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Ver también

* class [RichText](../)
* espacio de nombres [Aspose.Note](../../richtext/)
* asamblea [Aspose.Note](../../../)


