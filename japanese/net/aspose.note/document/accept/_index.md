---
title: Document.Accept
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. ノードの訪問者を受け入れます
type: docs
weight: 80
url: /ja/net/aspose.note/document/accept/
---
## Document.Accept method

ノードの訪問者を受け入れます。

```csharp
public override void Accept(DocumentVisitor visitor)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| visitor | DocumentVisitor | から派生したクラスのオブジェクト[`DocumentVisitor`](../../documentvisitor/). |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


