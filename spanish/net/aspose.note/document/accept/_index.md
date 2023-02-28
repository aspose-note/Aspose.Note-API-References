---
title: Document.Accept
second_title: Aspose.Note para la referencia de la API de .NET
description: Document método. Acepta al visitante del nodo.
type: docs
weight: 80
url: /es/net/aspose.note/document/accept/
---
## Document.Accept method

Acepta al visitante del nodo.

```csharp
public override void Accept(DocumentVisitor visitor)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| visitor | DocumentVisitor | El objeto de una clase derivada de la[`DocumentVisitor`](../../documentvisitor/) . |

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

* class [DocumentVisitor](../../documentvisitor/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


