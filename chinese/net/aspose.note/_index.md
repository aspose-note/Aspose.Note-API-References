---
title: "Aspose.Note"
second_title: "Aspose.Note for .NET API 参考"
description: "该 Note 命名空间包含表示文档结构的类"
type: docs
weight: 10
url: /zh/net/aspose.note/
---
Note 命名空间包含表示文档结构的类。

## 类

| 类 | 描述 |
| --- | --- |
| [AttachedFile](./attachedfile/) | 表示一个附加文件。 |
| [CheckBox](./checkbox/) | 用于在完成和未完成之间切换状态的标签的基类。 |
| [CompositeNode&lt;T&gt;](./compositenode-1/) | 可以包含其他节点的节点的基泛型类。 |
| [CompositeNodeBase](./compositenodebase/) | 可以包含其他节点的节点的非泛型类。 |
| [DisplayUnitsConverter](./displayunitsconverter/) | 该类包含用于转换值的方法。 |
| [Document](./document/) | 表示一个 Aspose.Note 文档。 |
| [DocumentVisitor](./documentvisitor/) | 用于遍历以指定节点为根的子树的抽象类。 |
| [FileCorruptedException](./filecorruptedexception/) | 在文档加载期间抛出，当文档似乎已损坏且无法加载时。 |
| [Image](./image/) | 表示一个图像。 |
| [IncorrectDocumentStructureException](./incorrectdocumentstructureexception/) | 如果用户创建的文档结构不正确，则抛出。 |
| [IncorrectPasswordException](./incorrectpasswordexception/) | 如果文档使用密码加密且打开文档时指定的密码不正确或缺失，则抛出。 |
| [IndentatedNode&lt;T&gt;](./indentatednode-1/) | 具有子节点相对缩进的节点的基类。 |
| [InkDrawing](./inkdrawing/) | 表示包含任何绘制内容的 ink 节点。 |
| [InkNode](./inknode/) | 表示所有 ink 节点的通用接口。 |
| [InkParagraph](./inkparagraph/) | 表示包含手写文本且具有倾斜书写等附加属性的 ink 节点。 |
| [InkWord](./inkword/) | 表示包含手写文本的 ink 节点。 |
| [License](./license/) | 提供对组件进行授权的方法。 |
| [LoadOptions](./loadoptions/) | 用于加载文档的选项。 |
| [Loop](./loop/) | 表示一个循环。 |
| [MergeOptions](./mergeoptions/) | 用于合并页面集合的选项。 |
| [Metered](./metered/) | 提供设置计量密钥的方法。 |
| [Node](./node/) | Aspose.Note 文档中所有节点的基类。 |
| [Notebook](./notebook/) | 表示一个 Aspose.Note 笔记本。 |
| [NotebookLoadOptions](./notebookloadoptions/) | 用于加载笔记本的选项。 |
| [NoteCheckBox](./notecheckbox/) | 表示可以在完成和未完成状态之间切换的笔记标签。 |
| [NoteTag](./notetag/) | 表示笔记标签。 |
| [NoteTask](./notetask/) | 表示笔记任务。 |
| [NumberList](./numberlist/) | 表示编号或项目符号列表。 |
| [Outline](./outline/) | 表示大纲。 |
| [OutlineElement](./outlineelement/) | 表示大纲元素。 |
| [OutlineGroup](./outlinegroup/) | 表示大纲组。 |
| [Page](./page/) | 表示页面。 |
| [PageHistory](./pagehistory/) | 表示页面历史。 |
| [ParagraphStyle](./paragraphstyle/) | 如果在 Styles 集合中没有匹配的 TextStyle 对象，或者此对象未指定所需设置，则使用的文本样式设置。 |
| [ParsingErrorInfo](./parsingerrorinfo/) | 有关解析期间发生的错误的信息。 |
| [RevisionSummary](./revisionsummary/) | 表示节点修订的摘要。 |
| [RichText](./richtext/) | 表示富文本。 |
| [Style](./style/) | 此类包含 [`ParagraphStyle`](../aspose.note/paragraphstyle/) 和 [`TextStyle`](../aspose.note/textstyle/) 类的公共属性。 |
| [Table](./table/) | 表示表格。 |
| [TableCell](./tablecell/) | 表示表格单元格。 |
| [TableColumn](./tablecolumn/) | 表示表格列。 |
| [TableRow](./tablerow/) | 表示表格行。 |
| [TextRun](./textrun/) | 表示带有关联样式的文本片段的类。 |
| [TextStyle](./textstyle/) | 指定文本样式。 |
| [Title](./title/) | 表示标题。 |
| [UnsupportedFileFormatException](./unsupportedfileformatexception/) | 在文档加载期间抛出，当文件格式未被识别或不受 Aspose.Note 支持时。 |
| [UnsupportedSaveFormatException](./unsupportedsaveformatexception/) | 如果请求的保存格式不受支持，则抛出。 |
## Structures

| 结构 | 描述 |
| --- | --- |
| [Margins](./margins/) | 指定节点边距的尺寸。 |
## 接口

| 接口 | 描述 |
| --- | --- |
| [ICompositeNode](./icompositenode/) | 用于可以包含其他节点的节点的接口。 |
| [ICompositeNode&lt;T&gt;](./icompositenode-1/) | 用于可以包含其他节点的节点的接口。 |
| [IIndentatedNode](./iindentatednode/) | 用于子节点具有相对缩进的节点的接口。 |
| [INode](./inode/) | 用于 Aspose.Note 文档中所有节点的接口。 |
| [INotebookChildNode](./inotebookchildnode/) | 表示 Aspose.Note 笔记本的子项。 |
| [INoteTag](./inotetag/) | 用于注释标签（即未关联 Outlook 任务的标签）的接口。 |
| [IOutlineChildNode](./ioutlinechildnode/) | 用于大纲节点所有子节点的接口。 |
| [IOutlineElementChildNode](./ioutlineelementchildnode/) | 用于大纲元素节点所有子节点的接口。 |
| [IPageChildNode](./ipagechildnode/) | 用于页面节点所有子节点的接口。 |
| [ITag](./itag/) | 用于各种标签的接口。 |
| [ITaggable](./itaggable/) | 用于可以被标签标记的节点的接口。 |
## 枚举

| 枚举 | 描述 |
| --- | --- |
| [FileFormat](./fileformat/) | 表示 OneNote 文件格式。 |
| [HorizontalAlignment](./horizontalalignment/) | 指定对齐方式。 |
| [NodeType](./nodetype/) | 指定节点的类型。 |
| [NumberFormat](./numberformat/) | 指定可用于一组自动编号对象的编号格式。完整列表请参阅 [MSDN](https://msdn.microsoft.com/en-us/library/dd923798(v=office.12).aspx) |
| [PageSizeType](./pagesizetype/) | 指定页面节点类型的大小。 |
| [SaveFormat](./saveformat/) | 指示文档保存的格式。 |
| [TagIcon](./tagicon/) | 指定标签或任务的图标。 |
| [TagStatus](./tagstatus/) | 指定注释标签节点的状态。 |


