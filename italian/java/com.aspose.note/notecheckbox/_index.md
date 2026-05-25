---
title: "NoteCheckBox"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un tag di nota che può alternare il suo stato tra completo e incompleto."
type: docs
weight: 53
url: /it/java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

Rappresenta un tag di nota che può alternare il suo stato tra completo e incompleto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | * Crea un nuovo tag di nota con l'icona BlueCheckBoxEmpty e l'etichetta predefinita. |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con l'icona BlueCheckBoxEmpty e l'etichetta specificata. |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | * Crea un nuovo tag di nota con l'icona BlueCheckBox1Empty e l'etichetta predefinita. |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | * Crea una nuova casella di controllo della nota con l'icona BlueCheckBox1Empty e l'etichetta specificata. |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | * Crea un nuovo tag di nota con l'icona BlueCheckBox2Empty e l'etichetta predefinita. |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | * Crea una nuova casella di controllo della nota con l'icona BlueCheckBox2Empty e l'etichetta specificata. |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | * Crea un nuovo tag di nota con l'icona BlueCheckBox3Empty e l'etichetta predefinita. |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | * Crea una nuova casella di controllo della nota con l'icona BlueCheckBox3Empty e l'etichetta specificata. |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | * Crea un nuovo tag di nota con l'icona BlueExclamationCheckBoxEmpty e l'etichetta predefinita. |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con l'icona BlueExclamationCheckBoxEmpty e l'etichetta specificata. |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | * Crea un nuovo tag di nota con l'icona BlueFlagCheckBoxEmpty e l'etichetta predefinita. |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con l'icona BlueFlagCheckBoxEmpty e l'etichetta specificata. |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | \* Crea un nuovo tag di nota con l'icona BluePersonCheckBoxEmpty e l'etichetta predefinita. |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona BluePersonCheckBoxEmpty e l'etichetta specificata. |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | \* Crea un nuovo tag di nota con l'icona BlueRightArrowCheckBoxEmpty e l'etichetta predefinita. |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona BlueRightArrowCheckBoxEmpty e l'etichetta specificata. |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | \* Crea un nuovo tag di nota con l'icona BlueStarCheckBoxEmpty e l'etichetta predefinita. |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona BlueStarCheckBoxEmpty e l'etichetta specificata. |
| [createGreenCheckBox()](#createGreenCheckBox--) | \* Crea un nuovo tag di nota con l'icona GreenCheckBoxEmpty e l'etichetta predefinita. |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenCheckBoxEmpty e l'etichetta specificata. |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | \* Crea un nuovo tag di nota con l'icona GreenCheckBox1Empty e l'etichetta predefinita. |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenCheckBox1Empty e l'etichetta specificata. |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | \* Crea un nuovo tag di nota con l'icona GreenCheckBox2Empty e l'etichetta predefinita. |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenCheckBox2Empty e l'etichetta specificata. |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | \* Crea un nuovo tag di nota con l'icona GreenCheckBox3Empty e l'etichetta predefinita. |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenCheckBox3Empty e l'etichetta specificata. |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | \* Crea un nuovo tag di nota con l'icona GreenExclamationCheckBoxEmpty e l'etichetta predefinita. |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenExclamationCheckBoxEmpty e l'etichetta specificata. |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | \* Crea un nuovo tag di nota con l'icona GreenFlagCheckBoxEmpty e l'etichetta predefinita. |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenFlagCheckBoxEmpty e l'etichetta specificata. |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | \* Crea un nuovo tag di nota con l'icona GreenPersonCheckBoxEmpty e l'etichetta predefinita. |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenPersonCheckBoxEmpty e l'etichetta specificata. |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | \* Crea un nuovo tag di nota con l'icona GreenRightArrowCheckBoxEmpty e l'etichetta predefinita. |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenRightArrowCheckBoxEmpty e l'etichetta specificata. |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | \* Crea un nuovo tag di nota con l'icona GreenStarCheckBoxEmpty e l'etichetta predefinita. |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | \* Crea una nuova casella di spunta di nota con l'icona GreenStarCheckBoxEmpty e l'etichetta specificata. |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | \* Crea un nuovo tag di nota con l'icona RedFlagCheckBoxEmpty e l'etichetta predefinita. |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona RedFlagCheckBoxEmpty e etichetta specificata. |
| [createYellowCheckBox()](#createYellowCheckBox--) | * Crea un nuovo tag della nota con icona YellowCheckBoxEmpty e etichetta predefinita. |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowCheckBoxEmpty e etichetta specificata. |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | * Crea un nuovo tag della nota con icona YellowCheckBox1Empty e etichetta predefinita. |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowCheckBox1Empty e etichetta specificata. |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | * Crea un nuovo tag della nota con icona YellowCheckBox2Empty e etichetta predefinita. |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowCheckBox2Empty e etichetta specificata. |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | * Crea un nuovo tag della nota con icona YellowCheckBox3Empty e etichetta predefinita. |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowCheckBox3Empty e etichetta specificata. |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | * Crea un nuovo tag della nota con icona YellowExclamationCheckBoxEmpty e etichetta predefinita. |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowExclamationCheckBoxEmpty e etichetta specificata. |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | * Crea un nuovo tag della nota con icona YellowPersonCheckBoxEmpty e etichetta predefinita. |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowPersonCheckBoxEmpty e etichetta specificata. |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | * Crea un nuovo tag della nota con icona YellowRightArrowCheckBoxEmpty e etichetta predefinita. |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowRightArrowCheckBoxEmpty e etichetta specificata. |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | * Crea un nuovo tag della nota con icona YellowStarCheckBoxEmpty e etichetta predefinita. |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | * Crea una nuova casella di controllo della nota con icona YellowStarCheckBoxEmpty e etichetta specificata. |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [getFontColor()](#getFontColor--) | Ottiene o imposta il colore del carattere. |
| [getHighlight()](#getHighlight--) | Ottiene o imposta il colore di evidenziazione. |
| [getIcon()](#getIcon--) | Ottiene o imposta l'icona. |
| [getLabel()](#getLabel--) | Ottiene o imposta il testo dell'etichetta. |
| [hashCode()](#hashCode--) | Funziona come funzione hash per il tipo. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Ottiene o imposta il colore del carattere. |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | Ottiene o imposta il colore di evidenziazione. |
| [setLabel(String value)](#setLabel-java.lang.String-) | Ottiene o imposta il testo dell'etichetta. |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


* Crea un nuovo tag di nota con l'icona BlueCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con l'icona BlueCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


* Crea un nuovo tag di nota con l'icona BlueCheckBox1Empty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


* Crea una nuova casella di controllo della nota con l'icona BlueCheckBox1Empty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


* Crea un nuovo tag di nota con l'icona BlueCheckBox2Empty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


* Crea una nuova casella di controllo della nota con l'icona BlueCheckBox2Empty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


* Crea un nuovo tag di nota con l'icona BlueCheckBox3Empty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


* Crea una nuova casella di controllo della nota con l'icona BlueCheckBox3Empty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


* Crea un nuovo tag di nota con l'icona BlueExclamationCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con l'icona BlueExclamationCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


* Crea un nuovo tag di nota con l'icona BlueFlagCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con l'icona BlueFlagCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


\* Crea un nuovo tag di nota con l'icona BluePersonCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona BluePersonCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


\* Crea un nuovo tag di nota con l'icona BlueRightArrowCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona BlueRightArrowCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


\* Crea un nuovo tag di nota con l'icona BlueStarCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona BlueStarCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


\* Crea un nuovo tag di nota con l'icona GreenCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


\* Crea un nuovo tag di nota con l'icona GreenCheckBox1Empty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenCheckBox1Empty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


\* Crea un nuovo tag di nota con l'icona GreenCheckBox2Empty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenCheckBox2Empty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


\* Crea un nuovo tag di nota con l'icona GreenCheckBox3Empty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenCheckBox3Empty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


\* Crea un nuovo tag di nota con l'icona GreenExclamationCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenExclamationCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


\* Crea un nuovo tag di nota con l'icona GreenFlagCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenFlagCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


\* Crea un nuovo tag di nota con l'icona GreenPersonCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenPersonCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


\* Crea un nuovo tag di nota con l'icona GreenRightArrowCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenRightArrowCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


\* Crea un nuovo tag di nota con l'icona GreenStarCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


\* Crea una nuova casella di spunta di nota con l'icona GreenStarCheckBoxEmpty e l'etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


\* Crea un nuovo tag di nota con l'icona RedFlagCheckBoxEmpty e l'etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con icona RedFlagCheckBoxEmpty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


* Crea un nuovo tag della nota con icona YellowCheckBoxEmpty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowCheckBoxEmpty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


* Crea un nuovo tag della nota con icona YellowCheckBox1Empty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowCheckBox1Empty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


* Crea un nuovo tag della nota con icona YellowCheckBox2Empty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowCheckBox2Empty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


* Crea un nuovo tag della nota con icona YellowCheckBox3Empty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowCheckBox3Empty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


* Crea un nuovo tag della nota con icona YellowExclamationCheckBoxEmpty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowExclamationCheckBoxEmpty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


* Crea un nuovo tag della nota con icona YellowPersonCheckBoxEmpty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowPersonCheckBoxEmpty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


* Crea un nuovo tag della nota con icona YellowRightArrowCheckBoxEmpty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowRightArrowCheckBoxEmpty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


* Crea un nuovo tag della nota con icona YellowStarCheckBoxEmpty e etichetta predefinita.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


* Crea una nuova casella di controllo della nota con icona YellowStarCheckBoxEmpty e etichetta specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| etichetta | java.lang.String | L'etichetta del tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


Determina se l'oggetto specificato è uguale all'oggetto corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | L'oggetto. |

**Returns:**
boolean - Il `boolean`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se l'oggetto specificato è uguale all'oggetto corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto. |

**Returns:**
boolean - Il `boolean`.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Ottiene o imposta il colore del carattere.

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


Ottiene o imposta il colore di evidenziazione.

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


Ottiene o imposta l'icona.

Valore: Il [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


Ottiene o imposta il testo dell'etichetta.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funziona come funzione hash per il tipo.

**Returns:**
int - Il `int`.
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Ottiene o imposta il colore del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


Ottiene o imposta il colore di evidenziazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


Ottiene o imposta il testo dell'etichetta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

