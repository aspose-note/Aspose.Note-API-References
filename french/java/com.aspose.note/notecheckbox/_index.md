---
title: "NoteCheckBox"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente une étiquette de note pouvant basculer son état entre complet et incomplet."
type: docs
weight: 53
url: /fr/java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

Représente une étiquette de note pouvant basculer son état entre complet et incomplet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | \* Crée une nouvelle balise de note avec l'icône BlueCheckBoxEmpty et l'étiquette par défaut. |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | \* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBoxEmpty et l'étiquette spécifiée. |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | \* Crée une nouvelle balise de note avec l'icône BlueCheckBox1Empty et l'étiquette par défaut. |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | \* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBox1Empty et l'étiquette spécifiée. |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | \* Crée une nouvelle balise de note avec l'icône BlueCheckBox2Empty et l'étiquette par défaut. |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | \* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBox2Empty et l'étiquette spécifiée. |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | \* Crée une nouvelle balise de note avec l'icône BlueCheckBox3Empty et l'étiquette par défaut. |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | \* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBox3Empty et l'étiquette spécifiée. |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | \* Crée une nouvelle balise de note avec l'icône BlueExclamationCheckBoxEmpty et l'étiquette par défaut. |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | \* Crée une nouvelle case à cocher de note avec l'icône BlueExclamationCheckBoxEmpty et l'étiquette spécifiée. |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | \* Crée une nouvelle balise de note avec l'icône BlueFlagCheckBoxEmpty et l'étiquette par défaut. |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | \* Crée une nouvelle case à cocher de note avec l'icône BlueFlagCheckBoxEmpty et l'étiquette spécifiée. |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône BluePersonCheckBoxEmpty et le libellé par défaut. |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône BluePersonCheckBoxEmpty et le libellé spécifié. |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône BlueRightArrowCheckBoxEmpty et le libellé par défaut. |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône BlueRightArrowCheckBoxEmpty et le libellé spécifié. |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône BlueStarCheckBoxEmpty et le libellé par défaut. |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône BlueStarCheckBoxEmpty et le libellé spécifié. |
| [createGreenCheckBox()](#createGreenCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône GreenCheckBoxEmpty et le libellé par défaut. |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenCheckBoxEmpty et le libellé spécifié. |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | * Crée une nouvelle étiquette de note avec l'icône GreenCheckBox1Empty et le libellé par défaut. |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenCheckBox1Empty et le libellé spécifié. |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | * Crée une nouvelle étiquette de note avec l'icône GreenCheckBox2Empty et le libellé par défaut. |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenCheckBox2Empty et le libellé spécifié. |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | * Crée une nouvelle étiquette de note avec l'icône GreenCheckBox3Empty et le libellé par défaut. |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenCheckBox3Empty et le libellé spécifié. |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône GreenExclamationCheckBoxEmpty et le libellé par défaut. |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenExclamationCheckBoxEmpty et le libellé spécifié. |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône GreenFlagCheckBoxEmpty et le libellé par défaut. |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenFlagCheckBoxEmpty et le libellé spécifié. |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône GreenPersonCheckBoxEmpty et le libellé par défaut. |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenPersonCheckBoxEmpty et le libellé spécifié. |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône GreenRightArrowCheckBoxEmpty et le libellé par défaut. |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenRightArrowCheckBoxEmpty et le libellé spécifié. |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône GreenStarCheckBoxEmpty et le libellé par défaut. |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône GreenStarCheckBoxEmpty et le libellé spécifié. |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône RedFlagCheckBoxEmpty et le libellé par défaut. |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône RedFlagCheckBoxEmpty et le libellé spécifié. |
| [createYellowCheckBox()](#createYellowCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône YellowCheckBoxEmpty et le libellé par défaut. |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowCheckBoxEmpty et le libellé spécifié. |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | * Crée une nouvelle étiquette de note avec l'icône YellowCheckBox1Empty et le libellé par défaut. |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowCheckBox1Empty et le libellé spécifié. |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | * Crée une nouvelle étiquette de note avec l'icône YellowCheckBox2Empty et le libellé par défaut. |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowCheckBox2Empty et le libellé spécifié. |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | * Crée une nouvelle étiquette de note avec l'icône YellowCheckBox3Empty et le libellé par défaut. |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowCheckBox3Empty et le libellé spécifié. |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône YellowExclamationCheckBoxEmpty et le libellé par défaut. |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowExclamationCheckBoxEmpty et le libellé spécifié. |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône YellowPersonCheckBoxEmpty et le libellé par défaut. |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowPersonCheckBoxEmpty et le libellé spécifié. |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône YellowRightArrowCheckBoxEmpty et le libellé par défaut. |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowRightArrowCheckBoxEmpty et le libellé spécifié. |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | * Crée une nouvelle étiquette de note avec l'icône YellowStarCheckBoxEmpty et le libellé par défaut. |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | * Crée une nouvelle case à cocher de note avec l'icône YellowStarCheckBoxEmpty et le libellé spécifié. |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [getFontColor()](#getFontColor--) | Obtient ou définit la couleur de la police. |
| [getHighlight()](#getHighlight--) | Obtient ou définit la couleur de surlignage. |
| [getIcon()](#getIcon--) | Obtient ou définit l'icône. |
| [getLabel()](#getLabel--) | Obtient ou définit le texte du libellé. |
| [hashCode()](#hashCode--) | Servit de fonction de hachage pour le type. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Obtient ou définit la couleur de la police. |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | Obtient ou définit la couleur de surlignage. |
| [setLabel(String value)](#setLabel-java.lang.String-) | Obtient ou définit le texte du libellé. |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


\* Crée une nouvelle balise de note avec l'icône BlueCheckBoxEmpty et l'étiquette par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


\* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBoxEmpty et l'étiquette spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


\* Crée une nouvelle balise de note avec l'icône BlueCheckBox1Empty et l'étiquette par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


\* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBox1Empty et l'étiquette spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


\* Crée une nouvelle balise de note avec l'icône BlueCheckBox2Empty et l'étiquette par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


\* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBox2Empty et l'étiquette spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


\* Crée une nouvelle balise de note avec l'icône BlueCheckBox3Empty et l'étiquette par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


\* Crée une nouvelle case à cocher de note avec l'icône BlueCheckBox3Empty et l'étiquette spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


\* Crée une nouvelle balise de note avec l'icône BlueExclamationCheckBoxEmpty et l'étiquette par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


\* Crée une nouvelle case à cocher de note avec l'icône BlueExclamationCheckBoxEmpty et l'étiquette spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


\* Crée une nouvelle balise de note avec l'icône BlueFlagCheckBoxEmpty et l'étiquette par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


\* Crée une nouvelle case à cocher de note avec l'icône BlueFlagCheckBoxEmpty et l'étiquette spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône BluePersonCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône BluePersonCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône BlueRightArrowCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône BlueRightArrowCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône BlueStarCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône BlueStarCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône GreenCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


* Crée une nouvelle étiquette de note avec l'icône GreenCheckBox1Empty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenCheckBox1Empty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


* Crée une nouvelle étiquette de note avec l'icône GreenCheckBox2Empty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenCheckBox2Empty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


* Crée une nouvelle étiquette de note avec l'icône GreenCheckBox3Empty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenCheckBox3Empty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône GreenExclamationCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenExclamationCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône GreenFlagCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenFlagCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône GreenPersonCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenPersonCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône GreenRightArrowCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenRightArrowCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône GreenStarCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône GreenStarCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône RedFlagCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône RedFlagCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône YellowCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


* Crée une nouvelle étiquette de note avec l'icône YellowCheckBox1Empty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowCheckBox1Empty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


* Crée une nouvelle étiquette de note avec l'icône YellowCheckBox2Empty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowCheckBox2Empty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


* Crée une nouvelle étiquette de note avec l'icône YellowCheckBox3Empty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowCheckBox3Empty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône YellowExclamationCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowExclamationCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône YellowPersonCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowPersonCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône YellowRightArrowCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowRightArrowCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


* Crée une nouvelle étiquette de note avec l'icône YellowStarCheckBoxEmpty et le libellé par défaut.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


* Crée une nouvelle case à cocher de note avec l'icône YellowStarCheckBoxEmpty et le libellé spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| libellé | java.lang.String | Le libellé de l'étiquette. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


Détermine si l'objet spécifié est égal à l'objet actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | L'objet. |

**Returns:**
booléen - Le `boolean`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si l'objet spécifié est égal à l'objet actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet. |

**Returns:**
booléen - Le `boolean`.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Obtient ou définit la couleur de la police.

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


Obtient ou définit la couleur de surlignage.

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


Obtient ou définit l'icône.

Valeur : Le [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


Obtient ou définit le texte du libellé.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Servit de fonction de hachage pour le type.

**Returns:**
int - Le `int`.
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Obtient ou définit la couleur de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


Obtient ou définit la couleur de surlignage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


Obtient ou définit le texte du libellé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

