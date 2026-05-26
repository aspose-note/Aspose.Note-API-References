---
title: "Document"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un documento Aspose.Note."
type: docs
weight: 20
url: /es/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Representa un documento Aspose.Note.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Document()](#Document--) | Inicializa una nueva instancia de la clase `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Inicializa una nueva instancia de la clase `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Inicializa una nueva instancia de la clase `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Inicializa una nueva instancia de la clase `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Inicializa una nueva instancia de la clase `Document`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Detecta todos los cambios realizados en el diseño del documento desde la llamada anterior a `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Obtiene un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente. |
| [getColor()](#getColor--) | Obtiene el color. |
| [getCreationTime()](#getCreationTime--) | Obtiene la hora de creación. |
| [getDisplayName()](#getDisplayName--) | Obtiene el nombre para mostrar. |
| [getFileFormat()](#getFileFormat--) | Obtiene el formato de archivo (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Obtiene el identificador único global del objeto. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Obtiene el `PageHistory` que contiene el historial completo de cada página presentada en un documento (la más antigua en el índice 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Comprueba si un documento proveniente de un flujo está cifrado. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Comprueba si un documento proveniente de un flujo está cifrado. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Comprueba si un documento proveniente de un flujo está cifrado. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Comprueba si un documento proveniente de un archivo está cifrado. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Comprueba si un documento proveniente de un archivo está cifrado. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Comprueba si un documento proveniente de un archivo está cifrado. |
| [print()](#print--) | Imprime el documento usando la impresora predeterminada. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Imprime el documento usando la impresora predeterminada. |
| [print(String printerName)](#print-java.lang.String-) | Imprime el documento usando la impresora predeterminada. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Imprime el documento usando la impresora predeterminada. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Guarda el documento OneNote en un flujo. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Guarda el documento OneNote en un flujo usando las opciones de guardado especificadas. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Guarda el documento OneNote en un flujo en el formato especificado. |
| [save(String fileName)](#save-java.lang.String-) | Guarda el documento OneNote en un archivo. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Guarda el documento OneNote en un archivo usando las opciones de guardado especificadas. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Guarda el documento OneNote en un archivo en el formato especificado. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Establece un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Establece el color. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Establece la hora de creación. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Establece el nombre para mostrar. |
### Document() {#Document--}
```
public Document()
```


Inicializa una nueva instancia de la clase `Document`. Crea un documento OneNote en blanco.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Inicializa una nueva instancia de la clase `Document`. Abre un documento OneNote existente desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase `Document`. Abre un documento OneNote existente desde un archivo. Permite especificar opciones adicionales como una contraseña de cifrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opciones usadas para cargar un documento. Puede ser nulo. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Inicializa una nueva instancia de la clase `Document`. Abre un documento OneNote existente desde un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inStream | java.io.InputStream | El flujo. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase `Document`. Abre un documento OneNote existente desde un flujo. Permite especificar opciones adicionales como una contraseña de cifrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inStream | java.io.InputStream | El flujo. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opciones usadas para cargar un documento. Puede ser nulo. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Detecta todos los cambios realizados en el diseño del documento desde la llamada anterior a `DetectLayoutChanges`. En caso de que `AutomaticLayoutChangesDetectionEnabled` esté configurado en true, se usa automáticamente al inicio de la exportación del documento.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Obtiene un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente. El valor predeterminado es `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Obtiene el color.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Obtiene la hora de creación.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtiene el nombre para mostrar.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Obtiene el formato de archivo (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Obtiene el identificador único global del objeto.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Obtiene el `PageHistory` que contiene el historial completo de cada página presentada en un documento (la más antigua en el índice 0). La revisión actual de la página se puede acceder como `PageHistory.current` y se almacena por separado de la colección de versiones históricas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | La revisión actual de una página. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Comprueba si un documento proveniente de un flujo está cifrado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede generar una penalización de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo. |
| document | [Document\[\]](../../com.aspose.note/document) | El documento cargado. |

**Returns:**
boolean - Devuelve true si el documento está cifrado, de lo contrario false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Comprueba si un documento proveniente de un flujo está cifrado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede generar una penalización de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Las opciones de carga. |
| document | [Document\[\]](../../com.aspose.note/document) | El documento cargado. |

**Returns:**
boolean - Devuelve true si el documento está cifrado, de lo contrario false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Comprueba si un documento proveniente de un flujo está cifrado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede generar una penalización de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo. |
| password | java.lang.String | La contraseña para descifrar un documento. |
| document | [Document\[\]](../../com.aspose.note/document) | El documento cargado. |

**Returns:**
boolean - Devuelve true si el documento está cifrado, de lo contrario false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Comprueba si un documento proveniente de un archivo está cifrado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede generar una penalización de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| document | [Document\[\]](../../com.aspose.note/document) | El documento cargado. |

**Returns:**
boolean - Devuelve true si el documento está cifrado, de lo contrario false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Comprueba si un documento proveniente de un archivo está cifrado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede generar una penalización de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Las opciones de carga. |
| document | [Document\[\]](../../com.aspose.note/document) | El documento cargado. |

**Returns:**
boolean - Devuelve true si el documento está cifrado, de lo contrario false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Comprueba si un documento proveniente de un archivo está cifrado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede generar una penalización de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo. |
| password | java.lang.String | La contraseña para descifrar un documento. |
| document | [Document\[\]](../../com.aspose.note/document) | El documento cargado. |

**Returns:**
boolean - Devuelve true si el documento está cifrado, de lo contrario false.
### print() {#print--}
```
public void print()
```


Imprime el documento usando la impresora predeterminada.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Imprime el documento usando la impresora predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Opciones usadas para imprimir un documento. Puede ser nulo. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Imprime el documento usando la impresora predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Imprime el documento usando la impresora predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Guarda el documento OneNote en un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | El System.iO.stream donde se guardará el documento. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Guarda el documento OneNote en un flujo usando las opciones de guardado especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | El System.iO.stream donde se guardará el documento. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Especifica las opciones de cómo se guarda el documento en el stream. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Guarda el documento OneNote en un flujo en el formato especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | El System.iO.stream donde se guardará el documento. |
| format | int | El formato en el que guardar el documento. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Guarda el documento OneNote en un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, el archivo existente se sobrescribe. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Guarda el documento OneNote en un archivo usando las opciones de guardado especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, el archivo existente se sobrescribe. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Especifica las opciones de cómo se guarda el documento en el archivo. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Guarda el documento OneNote en un archivo en el formato especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombreArchivo | java.lang.String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, el archivo existente se sobrescribe. |
| format | int | El formato en el que guardar el documento. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Establece un valor que indica si Aspose.Note realiza la detección de cambios de diseño automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | Nuevo valor. Puede ser nulo. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Establece el color.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | Valor del Color. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Establece la hora de creación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | Valor del DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Establece el nombre para mostrar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | Valor del DateTime. |

