---
title: Class CheckBox
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.CheckBox clase. La clase base para etiquetas que pueden alternar su estado entre completo e incompleto.
type: docs
weight: 20
url: /es/net/aspose.note/checkbox/
---
## CheckBox class

La clase base para etiquetas que pueden alternar su estado entre completo e incompleto.

```csharp
public abstract class CheckBox : ITag
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Obtiene un valor que indica si CheckBox está en estado marcado. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Obtiene o establece el tiempo completado. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Obtiene o establece la hora de creación. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Obtiene o establece el icono. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Obtiene el texto de la etiqueta. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Obtiene o establece el estado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Establece la etiqueta en estado completado utilizando la hora actual como hora completada. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Establece la etiqueta en estado completado. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Establece la etiqueta en estado abierto. |

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

Muestra cómo completar todos los elementos de la casilla de verificación relacionados con el 'Proyecto C'.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
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

Muestra cómo abrir todas las casillas de verificación relacionadas con el 'Proyecto C'.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

Muestra cómo generar un pdf que contenga páginas con elementos marcados con casillas de verificación incompletas y creado durante la semana pasada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

Muestra cómo generar un pdf que contenga páginas con tareas incompletas de Outlook para completar esta semana.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

### Ver también

* interface [ITag](../itag/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


