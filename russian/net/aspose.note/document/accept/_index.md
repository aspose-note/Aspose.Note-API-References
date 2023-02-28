---
title: Document.Accept
second_title: Справочник по API Aspose.Note для .NET
description: Document метод. Принимает посетителя узла.
type: docs
weight: 80
url: /ru/net/aspose.note/document/accept/
---
## Document.Accept method

Принимает посетителя узла.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | DocumentVisitor | Объект класса, производного от[`DocumentVisitor`](../../documentvisitor/) . |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


