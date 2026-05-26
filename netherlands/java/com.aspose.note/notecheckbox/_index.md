---
title: "NoteCheckBox"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een notitag voor die hun status kan schakelen tussen voltooid en onvoltooid."
type: docs
weight: 53
url: /nl/java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

Stelt een notitag voor die hun status kan schakelen tussen voltooid en onvoltooid.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | * Maakt een nieuw notitie‑tag met BlueCheckBoxEmpty‑pictogram en standaardlabel. |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met BlueCheckBoxEmpty‑pictogram en opgegeven label. |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | * Maakt een nieuw notitie‑tag met BlueCheckBox1Empty‑pictogram en standaardlabel. |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met BlueCheckBox1Empty‑pictogram en opgegeven label. |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | * Maakt een nieuw notitie‑tag met BlueCheckBox2Empty‑pictogram en standaardlabel. |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met BlueCheckBox2Empty‑pictogram en opgegeven label. |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | * Maakt een nieuw notitie‑tag met BlueCheckBox3Empty‑pictogram en standaardlabel. |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met BlueCheckBox3Empty‑pictogram en opgegeven label. |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | * Maakt een nieuw notitie‑tag met BlueExclamationCheckBoxEmpty‑pictogram en standaardlabel. |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met BlueExclamationCheckBoxEmpty‑pictogram en opgegeven label. |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | * Maakt een nieuw notitie‑tag met BlueFlagCheckBoxEmpty‑pictogram en standaardlabel. |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met BlueFlagCheckBoxEmpty‑pictogram en opgegeven label. |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | * Maakt een nieuw notitie‑tag met BluePersonCheckBoxEmpty pictogram en standaardlabel. |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met BluePersonCheckBoxEmpty pictogram en opgegeven label. |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | * Maakt een nieuw notitie‑tag met BlueRightArrowCheckBoxEmpty pictogram en standaardlabel. |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met BlueRightArrowCheckBoxEmpty pictogram en opgegeven label. |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | * Maakt een nieuw notitie‑tag met BlueStarCheckBoxEmpty pictogram en standaardlabel. |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met BlueStarCheckBoxEmpty pictogram en opgegeven label. |
| [createGreenCheckBox()](#createGreenCheckBox--) | * Maakt een nieuw notitie‑tag met GreenCheckBoxEmpty pictogram en standaardlabel. |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenCheckBoxEmpty pictogram en opgegeven label. |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | * Maakt een nieuw notitie‑tag met GreenCheckBox1Empty pictogram en standaardlabel. |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenCheckBox1Empty pictogram en opgegeven label. |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | * Maakt een nieuw notitie‑tag met GreenCheckBox2Empty pictogram en standaardlabel. |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenCheckBox2Empty pictogram en opgegeven label. |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | * Maakt een nieuw notitie‑tag met GreenCheckBox3Empty pictogram en standaardlabel. |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenCheckBox3Empty pictogram en opgegeven label. |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | * Maakt een nieuw notitie‑tag met GreenExclamationCheckBoxEmpty pictogram en standaardlabel. |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenExclamationCheckBoxEmpty pictogram en opgegeven label. |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | * Maakt een nieuw notitie‑tag met GreenFlagCheckBoxEmpty pictogram en standaardlabel. |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenFlagCheckBoxEmpty pictogram en opgegeven label. |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | * Maakt een nieuw notitie‑tag met GreenPersonCheckBoxEmpty pictogram en standaardlabel. |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenPersonCheckBoxEmpty pictogram en opgegeven label. |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | * Maakt een nieuw notitie‑tag met GreenRightArrowCheckBoxEmpty pictogram en standaardlabel. |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenRightArrowCheckBoxEmpty pictogram en opgegeven label. |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | * Maakt een nieuw notitie‑tag met GreenStarCheckBoxEmpty pictogram en standaardlabel. |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑checkbox met GreenStarCheckBoxEmpty pictogram en opgegeven label. |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | * Maakt een nieuw notitie‑tag met RedFlagCheckBoxEmpty pictogram en standaardlabel. |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met RedFlagCheckBoxEmpty‑pictogram en opgegeven label. |
| [createYellowCheckBox()](#createYellowCheckBox--) | * Maakt een nieuw notitie‑tag met YellowCheckBoxEmpty‑pictogram en standaardlabel. |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowCheckBoxEmpty‑pictogram en opgegeven label. |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | * Maakt een nieuw notitie‑tag met YellowCheckBox1Empty‑pictogram en standaardlabel. |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowCheckBox1Empty‑pictogram en opgegeven label. |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | * Maakt een nieuw notitie‑tag met YellowCheckBox2Empty‑pictogram en standaardlabel. |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowCheckBox2Empty‑pictogram en opgegeven label. |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | * Maakt een nieuw notitie‑tag met YellowCheckBox3Empty‑pictogram en standaardlabel. |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowCheckBox3Empty‑pictogram en opgegeven label. |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | * Maakt een nieuw notitie‑tag met YellowExclamationCheckBoxEmpty‑pictogram en standaardlabel. |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowExclamationCheckBoxEmpty‑pictogram en opgegeven label. |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | * Maakt een nieuw notitie‑tag met YellowPersonCheckBoxEmpty‑pictogram en standaardlabel. |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowPersonCheckBoxEmpty‑pictogram en opgegeven label. |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | * Maakt een nieuw notitie‑tag met YellowRightArrowCheckBoxEmpty‑pictogram en standaardlabel. |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowRightArrowCheckBoxEmpty‑pictogram en opgegeven label. |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | * Maakt een nieuw notitie‑tag met YellowStarCheckBoxEmpty‑pictogram en standaardlabel. |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | * Maakt een nieuw notitie‑selectievakje met YellowStarCheckBoxEmpty‑pictogram en opgegeven label. |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [getFontColor()](#getFontColor--) | Haalt de letterkleur op of stelt deze in. |
| [getHighlight()](#getHighlight--) | Haalt de markeerkleur op of stelt deze in. |
| [getIcon()](#getIcon--) | Haalt het pictogram op of stelt dit in. |
| [getLabel()](#getLabel--) | Haalt de labeltekst op of stelt deze in. |
| [hashCode()](#hashCode--) | Dient als een hash-functie voor het type. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Haalt de letterkleur op of stelt deze in. |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | Haalt de markeerkleur op of stelt deze in. |
| [setLabel(String value)](#setLabel-java.lang.String-) | Haalt de labeltekst op of stelt deze in. |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


* Maakt een nieuw notitie‑tag met BlueCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met BlueCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


* Maakt een nieuw notitie‑tag met BlueCheckBox1Empty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


* Maakt een nieuw notitie‑selectievakje met BlueCheckBox1Empty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


* Maakt een nieuw notitie‑tag met BlueCheckBox2Empty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


* Maakt een nieuw notitie‑selectievakje met BlueCheckBox2Empty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


* Maakt een nieuw notitie‑tag met BlueCheckBox3Empty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


* Maakt een nieuw notitie‑selectievakje met BlueCheckBox3Empty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


* Maakt een nieuw notitie‑tag met BlueExclamationCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met BlueExclamationCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


* Maakt een nieuw notitie‑tag met BlueFlagCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met BlueFlagCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


* Maakt een nieuw notitie‑tag met BluePersonCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met BluePersonCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


* Maakt een nieuw notitie‑tag met BlueRightArrowCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met BlueRightArrowCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


* Maakt een nieuw notitie‑tag met BlueStarCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met BlueStarCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


* Maakt een nieuw notitie‑tag met GreenCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


* Maakt een nieuw notitie‑tag met GreenCheckBox1Empty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenCheckBox1Empty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


* Maakt een nieuw notitie‑tag met GreenCheckBox2Empty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenCheckBox2Empty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


* Maakt een nieuw notitie‑tag met GreenCheckBox3Empty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenCheckBox3Empty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


* Maakt een nieuw notitie‑tag met GreenExclamationCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenExclamationCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


* Maakt een nieuw notitie‑tag met GreenFlagCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenFlagCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


* Maakt een nieuw notitie‑tag met GreenPersonCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenPersonCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


* Maakt een nieuw notitie‑tag met GreenRightArrowCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenRightArrowCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


* Maakt een nieuw notitie‑tag met GreenStarCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


* Maakt een nieuw notitie‑checkbox met GreenStarCheckBoxEmpty pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


* Maakt een nieuw notitie‑tag met RedFlagCheckBoxEmpty pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met RedFlagCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


* Maakt een nieuw notitie‑tag met YellowCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


* Maakt een nieuw notitie‑tag met YellowCheckBox1Empty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowCheckBox1Empty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


* Maakt een nieuw notitie‑tag met YellowCheckBox2Empty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowCheckBox2Empty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


* Maakt een nieuw notitie‑tag met YellowCheckBox3Empty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowCheckBox3Empty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


* Maakt een nieuw notitie‑tag met YellowExclamationCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowExclamationCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


* Maakt een nieuw notitie‑tag met YellowPersonCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowPersonCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


* Maakt een nieuw notitie‑tag met YellowRightArrowCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowRightArrowCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


* Maakt een nieuw notitie‑tag met YellowStarCheckBoxEmpty‑pictogram en standaardlabel.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


* Maakt een nieuw notitie‑selectievakje met YellowStarCheckBoxEmpty‑pictogram en opgegeven label.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| label | java.lang.String | Het label van de tag. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


Bepaalt of het opgegeven object gelijk is aan het huidige object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | Het object. |

**Returns:**
boolean - De `boolean`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bepaalt of het opgegeven object gelijk is aan het huidige object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object. |

**Returns:**
boolean - De `boolean`.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Haalt de letterkleur op of stelt deze in.

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


Haalt de markeerkleur op of stelt deze in.

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


Haalt het pictogram op of stelt dit in.

Waarde: De [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


Haalt de labeltekst op of stelt deze in.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als een hash-functie voor het type.

**Returns:**
int - De `int`.
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Haalt de letterkleur op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


Haalt de markeerkleur op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


Haalt de labeltekst op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

