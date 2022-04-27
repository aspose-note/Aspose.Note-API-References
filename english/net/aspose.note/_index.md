---
title: Aspose.Note
second_title: Aspose.Note for .NET API Reference
description: The Note namespace contains classes which represent document structure.
type: docs
weight: 10
url: /net/aspose.note/
---
The Note namespace contains classes which represent document structure.

## Classes

| Class | Description |
| --- | --- |
| class [AttachedFile](./attachedfile) | Represents an attached file. |
| abstract class [CheckBox](./checkbox) | The base class for tags that can toggle their state between complete and incomplete. |
| abstract class [CompositeNode&lt;T&gt;](./compositenode-1) | The base generic class for nodes that can contain other nodes. |
| abstract class [CompositeNodeBase](./compositenodebase) | The non-generic class for nodes that can contain other nodes. |
| static class [DisplayUnitsConverter](./displayunitsconverter) | The class contains the methods for converting values. |
| class [Document](./document) | Represents an Aspose.Note document. |
| abstract class [DocumentVisitor](./documentvisitor) | The abstract class for iterating through subtree with root at the specified node. |
| class [FileCorruptedException](./filecorruptedexception) | Thrown during document load, when the document appears to be corrupted and impossible to load. |
| class [Image](./image) | Represents an Image. |
| class [IncorrectDocumentStructureException](./incorrectdocumentstructureexception) | Thrown if a user created document has incorrect structure. |
| class [IncorrectPasswordException](./incorrectpasswordexception) | Thrown if a document is encrypted with a password and the password specified when opening the document is incorrect or missing. |
| class [License](./license) | Provides methods to license the component. |
| class [LoadOptions](./loadoptions) | Options used to load a document. |
| abstract class [Node](./node) | The base class for all nodes of an Aspose.Note document. |
| class [Notebook](./notebook) | Represents an Aspose.Note notebook. |
| class [NotebookLoadOptions](./notebookloadoptions) | Options used to load a notebook. |
| class [NoteCheckBox](./notecheckbox) | Represents a note tag that can toggle their state between complete and incomplete. |
| class [NoteTag](./notetag) | Represents a note tag. |
| class [NoteTask](./notetask) | Represents a note task. |
| class [NumberList](./numberlist) | Represents the numbered or bulleted list. |
| class [Outline](./outline) | Represents a Outline. |
| class [OutlineElement](./outlineelement) | Represents a OutlineElement. |
| class [OutlineGroup](./outlinegroup) | Represents a OutlineGroup. |
| class [Page](./page) | Represents a page. |
| class [PageHistory](./pagehistory) | Represents the page history. |
| class [ParagraphStyle](./paragraphstyle) | Text style settings to be used if there is no matching TextStyle object in [`Styles`](aspose.note/richtext/styles) collection either this object doesn't specify a needed setting. |
| class [RevisionSummary](./revisionsummary) | Represents a summary for node's revision. |
| class [RichText](./richtext) | Represents a rich text. |
| class [Style](./style) | This class contains common properties of [`ParagraphStyle`](aspose.note/paragraphstyle) and [`TextStyle`](aspose.note/textstyle) classes. |
| class [Table](./table) | Represents a table. |
| class [TableCell](./tablecell) | Represents a table cell. |
| class [TableColumn](./tablecolumn) | Represents a table column. |
| class [TableRow](./tablerow) | Represents a table row. |
| class [TextStyle](./textstyle) | Specifies the text style. |
| class [Title](./title) | Represents a title. |
| class [UnsupportedFileFormatException](./unsupportedfileformatexception) | Thrown during document load, when the file format is not recognized or not supported by Aspose.Note. |
| class [UnsupportedSaveFormatException](./unsupportedsaveformatexception) | Thrown if requested save format is not supported. |
## Interfaces

| Interface | Description |
| --- | --- |
| interface [ICompositeNode](./icompositenode) | The interface for nodes that can contain other nodes. |
| interface [ICompositeNode&lt;T&gt;](./icompositenode-1) | The interface for nodes that can contain other nodes. |
| interface [INode](./inode) | The interface for all nodes of an Aspose.Note document. |
| interface [INotebookChildNode](./inotebookchildnode) | Represents an Aspose.Note notebook's child. |
| interface [INoteTag](./inotetag) | The interface for note tags(i.e. tags that are not associated with Outlook tasks). |
| interface [IOutlineChildNode](./ioutlinechildnode) | The interface for all child nodes of an outline node. |
| interface [IOutlineElementChildNode](./ioutlineelementchildnode) | The interface for all child nodes of an outline element node. |
| interface [IPageChildNode](./ipagechildnode) | The interface for all child nodes of a page node. |
| interface [ITag](./itag) | The interface for tags of all kinds. |
| interface [ITaggable](./itaggable) | The interface for nodes that can be marked by tags. |
## Enumeration

| Enumeration | Description |
| --- | --- |
| enum [FileFormat](./fileformat) | Represents OneNote file format. |
| enum [HorizontalAlignment](./horizontalalignment) | Specifies the alignment. |
| enum [NodeType](./nodetype) | Specifies the type of the node. |
| enum [NumberFormat](./numberformat) | Specifies the numbering format that can be used for a group of automatically numbered objects. Full list is specified on [MSDN](https://msdn.microsoft.com/en-us/library/dd923798(v=office.12).aspx) |
| enum [PageSizeType](./pagesizetype) | Specifies the size of the page node type. |
| enum [SaveFormat](./saveformat) | Indicates the format in which the document is saved. |
| enum [TagIcon](./tagicon) | Specifies the icon of tag or task icon. |
| enum [TagStatus](./tagstatus) | Specifies the status of the note tag node. |
| enum [TaskType](./tasktype) | Specifies the type of the note task node. |

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
