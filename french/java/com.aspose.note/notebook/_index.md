---
title: "Notebook"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un carnet Aspose.Note."
type: docs
weight: 56
url: /fr/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Représente un carnet Aspose.Note.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Notebook()](#Notebook--) | Initialise une nouvelle instance de la classe `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Initialise une nouvelle instance de la classe `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Initialise une nouvelle instance de la classe `Notebook`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Obtient tous les nœuds enfants par type de nœud. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Ajoute le nœud à la fin de la liste. |
| [getColor()](#getColor--) | Obtient ou définit la couleur. |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans le `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Obtient ou définit le nom d'affichage. |
| [getFileFormat()](#getFileFormat--) | Obtient le format de fichier (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Obtient l'identifiant unique global de l'objet. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Obtient le nœud enfant du bloc-notes à l'index donné. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Obtient ou définit une valeur indiquant si l'historique est activé. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt les nœuds enfants du `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Ajoute un nœud de document enfant. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Ajoute un nœud de document enfant. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Ajoute un nœud de document enfant. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Ajoute un nœud de document enfant. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Ajoute un nœud de bloc-notes enfant. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Ajoute un nœud de bloc-notes enfant. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Supprime le nœud enfant. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Enregistre le document OneNote dans un flux. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Enregistre le document OneNote dans un flux en utilisant les options d'enregistrement spécifiées. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Enregistre le document OneNote dans un flux au format spécifié. |
| [save(String fileName)](#save-java.lang.String-) | Enregistre le document OneNote dans un fichier. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Enregistre le document OneNote dans un fichier en utilisant les options d'enregistrement spécifiées. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Enregistre le document OneNote dans un fichier au format spécifié. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Obtient ou définit la couleur. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Obtient ou définit le nom d'affichage. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Obtient ou définit une valeur indiquant si l'historique est activé. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Initialise une nouvelle instance de la classe `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Initialise une nouvelle instance de la classe `Notebook`. Ouvre un bloc-notes OneNote existant à partir d'un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe `Notebook`. Ouvre un carnet OneNote existant à partir d'un fichier. Permet de spécifier des options supplémentaires telles qu'une stratégie de chargement des enfants ("lazy"/instant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Les options de chargement. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Obtient tous les nœuds enfants par type de nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Une liste de nœuds enfants.

`T1`: Le type des éléments dans la liste retournée.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Ajoute le nœud à la fin de la liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Le nœud à ajouter. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Obtient ou définit la couleur.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre d'éléments contenus dans le `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtient ou définit le nom d'affichage.

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

Valeur: Le GUID.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


Obtient le nœud enfant du bloc-notes à l'index donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Index du nœud enfant. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Obtient ou définit une valeur indiquant si l'historique est activé.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Renvoie un énumérateur qui parcourt les nœuds enfants du `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Un `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un flux. Permet de spécifier des options de chargement supplémentaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Le flux. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Les options de chargement. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Ajoute un nœud de document enfant. Ouvre un document OneNote existant à partir d'un fichier. Permet de spécifier des options de chargement supplémentaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Les options de chargement. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Ajoute un nœud de carnet enfant. Ouvre un carnet OneNote existant à partir d'un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Ajoute un nœud de carnet enfant. Ouvre un carnet OneNote existant à partir d'un fichier. Permet de spécifier des options de chargement supplémentaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Les options de chargement. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Supprime le nœud enfant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Le nœud à supprimer. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Enregistre le document OneNote dans un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | Le flux. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Enregistre le document OneNote dans un flux en utilisant les options d'enregistrement spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | Le flux. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Spécifie les options de sauvegarde du document. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Enregistre le document OneNote dans un flux au format spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | Le flux. |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Enregistre le document OneNote dans un fichier en utilisant les options d'enregistrement spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom complet du fichier. Si un fichier portant le nom complet spécifié existe déjà, le fichier existant est écrasé. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Spécifie les options de sauvegarde du document dans le fichier. |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Obtient ou définit la couleur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Obtient ou définit le nom d'affichage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Obtient ou définit une valeur indiquant si l'historique est activé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

