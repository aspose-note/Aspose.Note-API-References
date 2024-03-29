---
title: Interface ITaggable
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.ITaggable interface. The interface for nodes that can be marked by tags
type: docs
weight: 240
url: /net/aspose.note/itaggable/
---
## ITaggable interface

The interface for nodes that can be marked by tags.

```csharp
public interface ITaggable : INode
```

## Properties

| Name | Description |
| --- | --- |
| [Tags](../../aspose.note/itaggable/tags/) { get; } | Gets the list of all tags. |

## Examples

Shows how to generate a pdf containing all pages related to 'Project A'.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
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

Shows how to make completed all checkbox items related to 'Project C'.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
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

Shows how to make open all checkbox items related to 'Project C'.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
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

Shows how to generate a pdf containing pages with items marked by incomplete checkboxes and created during last week.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
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

Shows how to generate a pdf containing pages with Outlook incomplete tasks to complete on this week.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
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

### See Also

* interface [INode](../inode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


