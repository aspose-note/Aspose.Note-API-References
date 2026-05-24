---
title: "PageHistory"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente l'historique de la page."
type: docs
weight: 70
url: /fr/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Représente l'historique de la page.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Initialise une nouvelle instance de la classe `PageHistory`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Ajoute la version de page à la fin de `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Ajoute les versions de page à la fin de `PageHistory`. |
| [clear()](#clear--) | Efface l'historique des pages. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Détermine si l'historique des pages contient la version de page. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Copie les versions de page dans un tableau, en commençant à un indice particulier.. |
| [getCurrent()](#getCurrent--) | Obtient la version de page actuelle. |
| [get_Item(int index)](#get-Item-int-) | Obtient ou définit la version de page à l'indice spécifié de `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Détermine l'indice d'une version de page spécifique dans l'historique des pages. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Insère une version de page dans l'historique des pages. |
| [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si l'historique des pages est en lecture seule. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt les nœuds enfants de `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Supprime la version de page à l'indice spécifié de `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Supprime la version de page du `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Supprime une plage de versions de page du `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Obtient ou définit la version de page à l'indice spécifié de `PageHistory`. |
| [size()](#size--) | Obtient le nombre de versions de page dans l'historique des pages. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Initialise une nouvelle instance de la classe `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | La version de page actuelle. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Ajoute la version de page à la fin de `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La version de page. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Ajoute les versions de page à la fin de `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| éléments | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | La collection `IEnumerable\{Page\}` des versions de page. |

### clear() {#clear--}
```
public void clear()
```


Efface l'historique des pages.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Détermine si l'historique des pages contient la version de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La version de page. |

**Returns:**
booléen - Le `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Copie les versions de page dans un tableau, en commençant à un indice particulier..

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Le tableau cible. |
| arrayIndex | int | L'indice du tableau. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Obtient la version de page actuelle.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Obtient ou définit la version de page à l'indice spécifié de `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'indice. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Détermine l'indice d'une version de page spécifique dans l'historique des pages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La version de page. |

**Returns:**
int - Le `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Insère une version de page dans l'historique des pages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'indice. |
| item | [Page](../../com.aspose.note/page) | La version de page. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Obtient une valeur indiquant si l'historique des pages est en lecture seule.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Renvoie un énumérateur qui parcourt les nœuds enfants de `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - Le `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime la version de page à l'indice spécifié de `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'indice. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Supprime la version de page du `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La version de page. |

**Returns:**
booléen - Le `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Supprime une plage de versions de page du `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'indice. |
| count | int | Le nombre. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Obtient ou définit la version de page à l'indice spécifié de `PageHistory`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'indice. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Obtient le nombre de versions de page dans l'historique des pages.

**Returns:**
int
