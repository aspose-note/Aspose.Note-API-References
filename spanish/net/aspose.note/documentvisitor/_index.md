---
title: Class DocumentVisitor
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.DocumentVisitor clase. La clase abstracta para iterar a través del subárbol con raíz en el nodo especificado.
type: docs
weight: 70
url: /es/net/aspose.note/documentvisitor/
---
## DocumentVisitor class

La clase abstracta para iterar a través del subárbol con raíz en el nodo especificado.

```csharp
public abstract class DocumentVisitor
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [VisitAttachedFileEnd](../../aspose.note/documentvisitor/visitattachedfileend/)(AttachedFile) | Fin para visitar el[`AttachedFile`](../attachedfile/) nodo. |
| virtual [VisitAttachedFileStart](../../aspose.note/documentvisitor/visitattachedfilestart/)(AttachedFile) | Empezar a visitar el[`AttachedFile`](../attachedfile/) nodo. |
| virtual [VisitDocumentEnd](../../aspose.note/documentvisitor/visitdocumentend/)(Document) | Fin para visitar el[`Document`](../document/) nodo. |
| virtual [VisitDocumentStart](../../aspose.note/documentvisitor/visitdocumentstart/)(Document) | Empezar a visitar el[`Document`](../document/) nodo. |
| virtual [VisitImageEnd](../../aspose.note/documentvisitor/visitimageend/)(Image) | Fin para visitar el[`Image`](../image/) nodo. |
| virtual [VisitImageStart](../../aspose.note/documentvisitor/visitimagestart/)(Image) | Empezar a visitar el[`Image`](../image/) nodo. |
| virtual [VisitOutlineElementEnd](../../aspose.note/documentvisitor/visitoutlineelementend/)(OutlineElement) | Fin para visitar el[`OutlineElement`](../outlineelement/) nodo. |
| virtual [VisitOutlineElementStart](../../aspose.note/documentvisitor/visitoutlineelementstart/)(OutlineElement) | Empezar a visitar el[`OutlineElement`](../outlineelement/) nodo. |
| virtual [VisitOutlineEnd](../../aspose.note/documentvisitor/visitoutlineend/)(Outline) | Fin para visitar el[`Outline`](../outline/) nodo. |
| virtual [VisitOutlineGroupEnd](../../aspose.note/documentvisitor/visitoutlinegroupend/)(OutlineGroup) | Fin para visitar el[`OutlineGroup`](../outlinegroup/) nodo. |
| virtual [VisitOutlineGroupStart](../../aspose.note/documentvisitor/visitoutlinegroupstart/)(OutlineGroup) | Empezar a visitar el[`OutlineGroup`](../outlinegroup/) nodo. |
| virtual [VisitOutlineStart](../../aspose.note/documentvisitor/visitoutlinestart/)(Outline) | Empezar a visitar el[`Outline`](../outline/) nodo. |
| virtual [VisitPageEnd](../../aspose.note/documentvisitor/visitpageend/)(Page) | Fin para visitar el[`Page`](../page/) nodo. |
| virtual [VisitPageStart](../../aspose.note/documentvisitor/visitpagestart/)(Page) | Empezar a visitar el[`Page`](../page/) nodo. |
| virtual [VisitRichTextEnd](../../aspose.note/documentvisitor/visitrichtextend/)(RichText) | Fin para visitar el[`RichText`](../richtext/) nodo. |
| virtual [VisitRichTextStart](../../aspose.note/documentvisitor/visitrichtextstart/)(RichText) | Empezar a visitar el[`RichText`](../richtext/) nodo. |
| virtual [VisitTableCellEnd](../../aspose.note/documentvisitor/visittablecellend/)(TableCell) | Fin para visitar el[`TableCell`](../tablecell/) nodo. |
| virtual [VisitTableCellStart](../../aspose.note/documentvisitor/visittablecellstart/)(TableCell) | Empezar a visitar el[`TableCell`](../tablecell/) nodo. |
| virtual [VisitTableEnd](../../aspose.note/documentvisitor/visittableend/)(Table) | Fin para visitar el[`Table`](../table/) nodo. |
| virtual [VisitTableRowEnd](../../aspose.note/documentvisitor/visittablerowend/)(TableRow) | Fin para visitar el[`TableRow`](../tablerow/) nodo. |
| virtual [VisitTableRowStart](../../aspose.note/documentvisitor/visittablerowstart/)(TableRow) | Empezar a visitar el[`TableRow`](../tablerow/) nodo. |
| virtual [VisitTableStart](../../aspose.note/documentvisitor/visittablestart/)(Table) | Empezar a visitar el[`Table`](../table/) nodo. |
| virtual [VisitTitleEnd](../../aspose.note/documentvisitor/visittitleend/)(Title) | Fin para visitar el[`Title`](../title/) nodo. |
| virtual [VisitTitleStart](../../aspose.note/documentvisitor/visittitlestart/)(Title) | Empezar a visitar el[`Title`](../title/) nodo. |

### Ejemplos

Muestra cómo acceder al contenido de un documento utilizando el visitante.

```csharp
public static void Run()
{
    // La ruta al directorio de documentos.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Abre el documento que queremos convertir.
    Document doc = new Document(dataDir + "Aspose.one");

    // Crear un objeto que herede de la clase DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Este es el conocido patrón Visitante. Obtenga el modelo para aceptar un visitante.
    // El modelo iterará a través de sí mismo llamando a los métodos correspondientes
    // en el objeto visitante (esto se llama visita).
    //
    // Tenga en cuenta que cada nodo en el modelo de objetos tiene el método Aceptar, por lo que la visita
    // puede ejecutarse no solo para todo el documento, sino también para cualquier nodo del documento.
    doc.Accept(myConverter);

    // Una vez completada la visita, podemos recuperar el resultado de la operación,
    // que en este ejemplo, se ha acumulado en el visitante.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Implementación simple de guardar un documento en formato de texto sin formato. Implementado como Visitante.
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
    /// Obtiene el texto sin formato del documento que fue acumulado por el visitante.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Agrega texto a la salida actual. Respeta el indicador de salida activado/desactivado.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo RichText en el documento.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo Documento en el documento.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo de página en el documento.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Llamado cuando finaliza el procesamiento de un nodo de página.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo Título en el documento.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo de imagen en el documento.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo de OutlineGroup en el documento.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo Esquema en el documento.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Llamado cuando se encuentra un nodo OutlineElement en el documento.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Obtiene el conteo total de nodos por parte del Visitante
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

### Ver también

* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


