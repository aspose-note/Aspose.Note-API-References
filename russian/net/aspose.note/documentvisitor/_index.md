---
title: DocumentVisitor
second_title: Справочник по API Aspose.Note для .NET
description: Абстрактный класс для итерации по поддереву с корнем в указанном узле.
type: docs
weight: 70
url: /ru/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

Абстрактный класс для итерации по поддереву с корнем в указанном узле.

```csharp
public abstract class DocumentVisitor
```

## Методы

| Имя | Описание |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend)(AttachedFile) | End для посещения узла[`AttachedFile`](../attachedfile). |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart)(AttachedFile) | Начните посещать узел[`AttachedFile`](../attachedfile). |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend)(Document) | End для посещения узла[`Document`](../document). |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart)(Document) | Начните посещать узел[`Document`](../document). |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend)(Image) | End для посещения узла[`Image`](../image). |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart)(Image) | Начните посещать узел[`Image`](../image). |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend)(OutlineElement) | End для посещения узла[`OutlineElement`](../outlineelement). |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart)(OutlineElement) | Начните посещать узел[`OutlineElement`](../outlineelement). |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend)(Outline) | End для посещения узла[`Outline`](../outline). |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend)(OutlineGroup) | End для посещения узла[`OutlineGroup`](../outlinegroup). |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart)(OutlineGroup) | Начните посещать узел[`OutlineGroup`](../outlinegroup). |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart)(Outline) | Начните посещать узел[`Outline`](../outline). |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend)(Page) | End для посещения узла[`Page`](../page). |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart)(Page) | Начните посещать узел[`Page`](../page). |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend)(RichText) | End для посещения узла[`RichText`](../richtext). |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart)(RichText) | Начните посещать узел[`RichText`](../richtext). |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend)(TableCell) | End для посещения узла[`TableCell`](../tablecell). |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart)(TableCell) | Начните посещать узел[`TableCell`](../tablecell). |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend)(Table) | End для посещения узла[`Table`](../table). |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend)(TableRow) | End для посещения узла[`TableRow`](../tablerow). |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart)(TableRow) | Начните посещать узел[`TableRow`](../tablerow). |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart)(Table) | Начните посещать узел[`Table`](../table). |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend)(Title) | End для посещения узла[`Title`](../title). |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart)(Title) | Начните посещать узел[`Title`](../title). |

### Примеры

Показывает, как получить доступ к содержимому документа с помощью посетителя.

```csharp
public static void Run()
{
    // Путь к каталогу документов.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Откройте документ, который мы хотим преобразовать.
    Document doc = new Document(dataDir + "Aspose.one");

    // Создаем объект, наследуемый от класса DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Это хорошо известный шаблон Посетитель. Заставьте модель принять посетителя.
    // Модель будет перебирать сама себя, вызывая соответствующие методы
    // на объекте посетителя (это называется посещением).
    //
    // Обратите внимание, что каждый узел в объектной модели имеет метод Accept, поэтому посещение
    // может выполняться не только для всего документа, но и для любого узла в документе.
    doc.Accept(myConverter);

    // После завершения посещения мы можем получить результат операции,
    // что в этом примере накопилось у посетителя.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Простая реализация сохранения документа в текстовом формате. Реализовано как посетитель.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// Получает обычный текст документа, который накопил посетитель.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Добавляет текст к текущему выводу. Учитывает включенный/отключенный выходной флаг.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел RichText.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел Document.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел страницы.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Вызывается, когда обработка узла Page завершена.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел Title.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел изображения.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел OutlineGroup.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел Outline.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Вызывается, когда в документе встречается узел OutlineElement.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Получает общее количество узлов посетителя
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### Смотрите также

* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
