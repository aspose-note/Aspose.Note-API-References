---
title: "Document"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un document Aspose.Note."
type: docs
weight: 20
url: /fr/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Représente un document Aspose.Note.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Document()](#Document--) | Initialise une nouvelle instance de la classe `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Initialise une nouvelle instance de la classe `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Initialise une nouvelle instance de la classe `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Initialise une nouvelle instance de la classe `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Initialise une nouvelle instance de la classe `Document`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Détecte toutes les modifications apportées à la mise en page du document depuis l'appel précédent de `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Obtient une valeur indiquant si Aspose.Note effectue automatiquement la détection des changements de mise en page. |
| [getColor()](#getColor--) | Obtient la couleur. |
| [getCreationTime()](#getCreationTime--) | Obtient la date de création. |
| [getDisplayName()](#getDisplayName--) | Obtient le nom d'affichage. |
| [getFileFormat()](#getFileFormat--) | Obtient le format de fichier (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Obtient l'identifiant unique global de l'objet. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Obtient le `PageHistory` qui contient l'historique complet de chaque page présentée dans un document (la plus ancienne à l'index 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Vérifie si un document provenant d'un flux est chiffré. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Vérifie si un document provenant d'un flux est chiffré. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Vérifie si un document provenant d'un flux est chiffré. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Vérifie si un document provenant d'un fichier est chiffré. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Vérifie si un document provenant d'un fichier est chiffré. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Vérifie si un document provenant d'un fichier est chiffré. |
| [print()](#print--) | Imprime le document en utilisant l'imprimante par défaut. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Imprime le document en utilisant l'imprimante par défaut. |
| [print(String printerName)](#print-java.lang.String-) | Imprime le document en utilisant l'imprimante par défaut. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Imprime le document en utilisant l'imprimante par défaut. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Enregistre le document OneNote dans un flux. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Enregistre le document OneNote dans un flux en utilisant les options d'enregistrement spécifiées. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Enregistre le document OneNote dans un flux au format spécifié. |
| [save(String fileName)](#save-java.lang.String-) | Enregistre le document OneNote dans un fichier. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Enregistre le document OneNote dans un fichier en utilisant les options d'enregistrement spécifiées. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Enregistre le document OneNote dans un fichier au format spécifié. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Définit une valeur indiquant si Aspose.Note effectue la détection des changements de mise en page automatiquement. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Définit la couleur. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Définit l'heure de création. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Définit le nom d'affichage. |
### Document() {#Document--}
```
public Document()
```


Initialise une nouvelle instance de la classe `Document`. Crée un document OneNote vierge.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Initialise une nouvelle instance de la classe `Document`. Ouvre un document OneNote existant à partir d'un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe `Document`. Ouvre un document OneNote existant à partir d'un fichier. Permet de spécifier des options supplémentaires telles qu'un mot de passe de chiffrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Options utilisées pour charger un document. Peut être nul. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Initialise une nouvelle instance de la classe `Document`. Ouvre un document OneNote existant à partir d'un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inStream | java.io.InputStream | Le flux. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe `Document`. Ouvre un document OneNote existant à partir d'un flux. Permet de spécifier des options supplémentaires telles qu'un mot de passe de chiffrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inStream | java.io.InputStream | Le flux. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Options utilisées pour charger un document. Peut être nul. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Détecte tous les changements apportés à la mise en page du document depuis l'appel précédent de `DetectLayoutChanges`. Si `AutomaticLayoutChangesDetectionEnabled` est défini sur true, il est utilisé automatiquement au début de l'exportation du document.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Obtient une valeur indiquant si Aspose.Note effectue la détection des changements de mise en page automatiquement. La valeur par défaut est `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Obtient la couleur.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Obtient la date de création.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtient le nom d'affichage.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Obtient le format de fichier (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Obtient l'identifiant unique global de l'objet.

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


Obtient le `PageHistory` qui contient l'historique complet de chaque page présentée dans un document (la plus ancienne à l'index 0). La révision actuelle de la page peut être accédée via `PageHistory.current` et est stockée séparément de la collection des versions historiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | La révision actuelle d'une page. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Vérifie si un document provenant d'un flux est chiffré. Pour le vérifier, nous devons charger complètement ce document. Ainsi, cette méthode peut entraîner une pénalité de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux. |
| document | [Document\[\]](../../com.aspose.note/document) | Le document chargé. |

**Returns:**
booléen - Retourne true si le document est chiffré, sinon false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Vérifie si un document provenant d'un flux est chiffré. Pour le vérifier, nous devons charger complètement ce document. Ainsi, cette méthode peut entraîner une pénalité de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Les options de chargement. |
| document | [Document\[\]](../../com.aspose.note/document) | Le document chargé. |

**Returns:**
booléen - Retourne true si le document est chiffré, sinon false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Vérifie si un document provenant d'un flux est chiffré. Pour le vérifier, nous devons charger complètement ce document. Ainsi, cette méthode peut entraîner une pénalité de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux. |
| password | java.lang.String | Le mot de passe pour déchiffrer un document. |
| document | [Document\[\]](../../com.aspose.note/document) | Le document chargé. |

**Returns:**
booléen - Retourne true si le document est chiffré, sinon false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Vérifie si un document provenant d'un fichier est chiffré. Pour le vérifier, nous devons charger complètement ce document. Ainsi, cette méthode peut entraîner une pénalité de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| document | [Document\[\]](../../com.aspose.note/document) | Le document chargé. |

**Returns:**
booléen - Retourne true si le document est chiffré, sinon false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Vérifie si un document provenant d'un fichier est chiffré. Pour le vérifier, nous devons charger complètement ce document. Ainsi, cette méthode peut entraîner une pénalité de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Les options de chargement. |
| document | [Document\[\]](../../com.aspose.note/document) | Le document chargé. |

**Returns:**
booléen - Retourne true si le document est chiffré, sinon false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Vérifie si un document provenant d'un fichier est chiffré. Pour le vérifier, nous devons charger complètement ce document. Ainsi, cette méthode peut entraîner une pénalité de performance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| password | java.lang.String | Le mot de passe pour déchiffrer un document. |
| document | [Document\[\]](../../com.aspose.note/document) | Le document chargé. |

**Returns:**
booléen - Retourne true si le document est chiffré, sinon false.
### print() {#print--}
```
public void print()
```


Imprime le document en utilisant l'imprimante par défaut.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Imprime le document en utilisant l'imprimante par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Options utilisées pour imprimer un document. Peut être nul. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Imprime le document en utilisant l'imprimante par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Imprime le document en utilisant l'imprimante par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Enregistre le document OneNote dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | Le flux System.iO où le document sera enregistré. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Enregistre le document OneNote dans un flux en utilisant les options d'enregistrement spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | Le flux System.iO où le document sera enregistré. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Spécifie les options de la façon dont le document est enregistré dans le flux. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Enregistre le document OneNote dans un flux au format spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | Le flux System.iO où le document sera enregistré. |
| format | int | Le format dans lequel enregistrer le document. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Enregistre le document OneNote dans un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom complet du fichier. Si un fichier portant le nom complet spécifié existe déjà, le fichier existant est écrasé. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Enregistre le document OneNote dans un fichier en utilisant les options d'enregistrement spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom complet du fichier. Si un fichier portant le nom complet spécifié existe déjà, le fichier existant est écrasé. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Spécifie les options de sauvegarde du document dans le fichier. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Enregistre le document OneNote dans un fichier au format spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom complet du fichier. Si un fichier portant le nom complet spécifié existe déjà, le fichier existant est écrasé. |
| format | int | Le format dans lequel enregistrer le document. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Définit une valeur indiquant si Aspose.Note effectue la détection des changements de mise en page automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean | Nouvelle valeur. Peut être nul. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Définit la couleur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | Valeur de la couleur. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Définit l'heure de création.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | Valeur de DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Définit le nom d'affichage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | Valeur de DateTime. |

