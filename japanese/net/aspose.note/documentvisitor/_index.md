---
title: Class DocumentVisitor
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.DocumentVisitor クラス. 指定したノードをルートとするサブツリーを反復処理するための抽象クラス
type: docs
weight: 70
url: /ja/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

指定したノードをルートとするサブツリーを反復処理するための抽象クラス。

```csharp
public abstract class DocumentVisitor
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | 訪問終了[`AttachedFile`](../attachedfile/)node. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | を訪問し始めます[`AttachedFile`](../attachedfile/)node. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | 訪問終了[`Document`](../document/)node. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | を訪問し始めます[`Document`](../document/)node. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | 訪問終了[`Image`](../image/)node. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | を訪問し始めます[`Image`](../image/)node. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | 訪問終了[`OutlineElement`](../outlineelement/)node. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | を訪問し始めます[`OutlineElement`](../outlineelement/)node. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | 訪問終了[`Outline`](../outline/)node. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | 訪問終了[`OutlineGroup`](../outlinegroup/)node. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | を訪問し始めます[`OutlineGroup`](../outlinegroup/)node. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | を訪問し始めます[`Outline`](../outline/)node. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | 訪問終了[`Page`](../page/)node. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | を訪問し始めます[`Page`](../page/)node. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | 訪問終了[`RichText`](../richtext/)node. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | を訪問し始めます[`RichText`](../richtext/)node. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | 訪問終了[`TableCell`](../tablecell/)node. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | を訪問し始めます[`TableCell`](../tablecell/)node. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | 訪問終了[`Table`](../table/)node. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | 訪問終了[`TableRow`](../tablerow/)node. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | を訪問し始めます[`TableRow`](../tablerow/)node. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | を訪問し始めます[`Table`](../table/)node. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | 訪問終了[`Title`](../title/)node. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | を訪問し始めます[`Title`](../title/)node. |

### 例

ビジターを使用してドキュメントのコンテンツにアクセスする方法を示します。

```csharp
public static void Run()
{
    /// ドキュメント ディレクトリへのパス。
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    /// 変換するドキュメントを開きます。
    Document doc = new Document(dataDir + "Aspose.one");

    /// DocumentVisitor クラスから継承するオブジェクトを作成します。
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    /// これはよく知られている Visitor パターンです。訪問者を受け入れるモデルを取得します。
    /// モデルは、対応するメソッドを呼び出すことによってそれ自体を反復処理します
    /// 訪問者オブジェクト (これは訪問と呼ばれます)。
    ///
    /// オブジェクト モデルのすべてのノードに Accept メソッドがあることに注意してください。
    /// ドキュメント全体だけでなく、ドキュメント内の任意のノードに対して実行できます。
    doc.Accept(myConverter);

    /// 訪問が完了すると、操作の結果を取得できます。
    /// この例では、訪問者に蓄積されています。
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

//// <summary>
//// ドキュメントをプレーン テキスト形式で保存する単純な実装。ビジターとして実装されます。
//// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    //// <summary>
    //// 訪問者が蓄積したドキュメントの平文を取得します。
    //// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    //// <summary>
    //// 現在の出力にテキストを追加します。有効化/無効化された出力フラグを尊重します。
    //// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    //// <summary>
    //// ドキュメント内で RichText ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    //// <summary>
    //// ドキュメント内で Document ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で Page ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    //// <summary>
    //// Page ノードの処理が終了したときに呼び出されます。
    //// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    //// <summary>
    //// ドキュメント内で Title ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で Image ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で OutlineGroup ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で Outline ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    //// <summary>
    //// ドキュメント内で OutlineElement ノードが検出されたときに呼び出されます。
    //// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    //// <summary>
    //// 訪問者によるノードの総数を取得します
    //// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


