---
title: Class NoteTask
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.NoteTask clase. Representa una tarea de nota.
type: docs
weight: 400
url: /es/net/aspose.note/notetask/
---
## NoteTask class

Representa una tarea de nota.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Obtiene un valor que indica si CheckBox está en estado marcado. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Obtiene o establece el tiempo completado. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Obtiene o establece la hora de creación. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | Obtiene o establece la fecha de vencimiento. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | Obtiene o establece el icono. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Obtiene el texto de la etiqueta. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Obtiene o establece el estado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | Crea una nueva tarea de nota con el icono NoFollowUpDateFlag y la fecha de vencimiento especificada. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | Crea una nueva tarea de nota con el icono FollowUpNextWeekFlag. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | Crea una nueva tarea de nota con el icono FollowUpThisWeekFlag. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | Crea una nueva tarea de nota con el icono FollowUpTodayFlag. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | Crea una nueva tarea de nota con el icono FollowUpTomorrowFlag. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | Crea una nueva tarea de nota con el icono NoFollowUpDateFlag. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | Determina si el objeto especificado es igual al objeto actual. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | Determina si el objeto especificado es igual al objeto actual. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | Sirve como función hash para el tipo. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | Establece la etiqueta en estado completado utilizando la hora actual como hora completada. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | Establece la etiqueta en estado completado. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | Establece la etiqueta en estado abierto. |

### Ejemplos

Muestra cómo generar un pdf que contenga todas las páginas relacionadas con el 'Proyecto A'.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

Muestra cómo acceder a los detalles de las tareas de Outlook.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tasks();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener todos los nodos RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterar a través de cada nodo
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Recuperar propiedades
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Ver también

* class [CheckBox](../checkbox/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


