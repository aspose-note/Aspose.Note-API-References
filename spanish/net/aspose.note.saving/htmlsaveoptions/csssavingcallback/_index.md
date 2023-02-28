---
title: HtmlSaveOptions.CssSavingCallback
second_title: Aspose.Note para la referencia de la API de .NET
description: HtmlSaveOptions propiedad. Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar CSS.
type: docs
weight: 30
url: /es/net/aspose.note.saving/htmlsaveoptions/csssavingcallback/
---
## HtmlSaveOptions.CssSavingCallback property

Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar CSS.

```csharp
public ICssSavingCallback CssSavingCallback { get; set; }
```

### Ejemplos

Muestra cómo guardar un documento en formato html con el almacenamiento de todos los recursos (css/fuentes/imágenes) mediante el uso de devoluciones de llamada definidas por el usuario.

```csharp
// El siguiente código crea la carpeta 'documentFolder' que contiene document.html, la carpeta 'css' con el archivo 'style.css', la carpeta 'images' con imágenes y la carpeta 'fonts' con fuentes.
// El archivo 'style.css' contendrá al final la siguiente cadena "/* Esta línea se agrega a la transmisión manualmente por el usuario */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Ver también

* interface [ICssSavingCallback](../../../aspose.note.saving.html/icsssavingcallback/)
* class [HtmlSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../htmlsaveoptions/)
* asamblea [Aspose.Note](../../../)


