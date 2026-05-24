---
title: "NoteCheckBox"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt ein Notiz-Tag dar, das seinen Zustand zwischen erledigt und unerledigt umschalten kann."
type: docs
weight: 53
url: /de/java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

Stellt ein Notiz-Tag dar, das seinen Zustand zwischen erledigt und unerledigt umschalten kann.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | * Erstellt ein neues Notiz-Tag mit dem BlueCheckBoxEmpty‑Symbol und der Standardbeschriftung. |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBoxEmpty‑Symbol und der angegebenen Beschriftung. |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | * Erstellt ein neues Notiz-Tag mit dem BlueCheckBox1Empty‑Symbol und der Standardbeschriftung. |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBox1Empty‑Symbol und der angegebenen Beschriftung. |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | * Erstellt ein neues Notiz-Tag mit dem BlueCheckBox2Empty‑Symbol und der Standardbeschriftung. |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBox2Empty‑Symbol und der angegebenen Beschriftung. |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | * Erstellt ein neues Notiz-Tag mit dem BlueCheckBox3Empty‑Symbol und der Standardbeschriftung. |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBox3Empty‑Symbol und der angegebenen Beschriftung. |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | * Erstellt ein neues Notiz-Tag mit dem BlueExclamationCheckBoxEmpty‑Symbol und der Standardbeschriftung. |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueExclamationCheckBoxEmpty‑Symbol und der angegebenen Beschriftung. |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | * Erstellt ein neues Notiz-Tag mit dem BlueFlagCheckBoxEmpty‑Symbol und der Standardbeschriftung. |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueFlagCheckBoxEmpty‑Symbol und der angegebenen Beschriftung. |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | * Erstellt ein neues Notiz-Tag mit BluePersonCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit BluePersonCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | * Erstellt ein neues Notiz-Tag mit BlueRightArrowCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit BlueRightArrowCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | * Erstellt ein neues Notiz-Tag mit BlueStarCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit BlueStarCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createGreenCheckBox()](#createGreenCheckBox--) | * Erstellt ein neues Notiz-Tag mit GreenCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | * Erstellt ein neues Notiz-Tag mit GreenCheckBox1Empty Symbol und Standardbeschriftung. |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBox1Empty Symbol und angegebener Beschriftung. |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | * Erstellt ein neues Notiz-Tag mit GreenCheckBox2Empty Symbol und Standardbeschriftung. |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBox2Empty Symbol und angegebener Beschriftung. |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | * Erstellt ein neues Notiz-Tag mit GreenCheckBox3Empty Symbol und Standardbeschriftung. |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBox3Empty Symbol und angegebener Beschriftung. |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | * Erstellt ein neues Notiz-Tag mit GreenExclamationCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenExclamationCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | * Erstellt ein neues Notiz-Tag mit GreenFlagCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenFlagCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | * Erstellt ein neues Notiz-Tag mit GreenPersonCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenPersonCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | * Erstellt ein neues Notiz-Tag mit GreenRightArrowCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenRightArrowCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | * Erstellt ein neues Notiz-Tag mit GreenStarCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | * Erstellt ein neues Notiz-Kontrollkästchen mit GreenStarCheckBoxEmpty Symbol und angegebener Beschriftung. |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | * Erstellt ein neues Notiz-Tag mit RedFlagCheckBoxEmpty Symbol und Standardbeschriftung. |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit RedFlagCheckBoxEmpty‑Icon und angegebenem Label. |
| [createYellowCheckBox()](#createYellowCheckBox--) | \* Erstellt ein neues Notiz‑Tag mit YellowCheckBoxEmpty‑Icon und Standard‑Label. |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBoxEmpty‑Icon und angegebenem Label. |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | \* Erstellt ein neues Notiz‑Tag mit YellowCheckBox1Empty‑Icon und Standard‑Label. |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBox1Empty‑Icon und angegebenem Label. |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | \* Erstellt ein neues Notiz‑Tag mit YellowCheckBox2Empty‑Icon und Standard‑Label. |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBox2Empty‑Icon und angegebenem Label. |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | \* Erstellt ein neues Notiz‑Tag mit YellowCheckBox3Empty‑Icon und Standard‑Label. |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBox3Empty‑Icon und angegebenem Label. |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | \* Erstellt ein neues Notiz‑Tag mit YellowExclamationCheckBoxEmpty‑Icon und Standard‑Label. |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowExclamationCheckBoxEmpty‑Icon und angegebenem Label. |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | \* Erstellt ein neues Notiz‑Tag mit YellowPersonCheckBoxEmpty‑Icon und Standard‑Label. |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowPersonCheckBoxEmpty‑Icon und angegebenem Label. |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | \* Erstellt ein neues Notiz‑Tag mit YellowRightArrowCheckBoxEmpty‑Icon und Standard‑Label. |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowRightArrowCheckBoxEmpty‑Icon und angegebenem Label. |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | \* Erstellt ein neues Notiz‑Tag mit YellowStarCheckBoxEmpty‑Icon und Standard‑Label. |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | \* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowStarCheckBoxEmpty‑Icon und angegebenem Label. |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist. |
| [getFontColor()](#getFontColor--) | Liest oder setzt die Schriftfarbe. |
| [getHighlight()](#getHighlight--) | Liest oder setzt die Hervorhebungsfarbe. |
| [getIcon()](#getIcon--) | Liest oder setzt das Icon. |
| [getLabel()](#getLabel--) | Liest oder setzt den Label‑Text. |
| [hashCode()](#hashCode--) | Dient als Hash-Funktion für den Typ. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Liest oder setzt die Schriftfarbe. |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | Liest oder setzt die Hervorhebungsfarbe. |
| [setLabel(String value)](#setLabel-java.lang.String-) | Liest oder setzt den Label‑Text. |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


* Erstellt ein neues Notiz-Tag mit dem BlueCheckBoxEmpty‑Symbol und der Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBoxEmpty‑Symbol und der angegebenen Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


* Erstellt ein neues Notiz-Tag mit dem BlueCheckBox1Empty‑Symbol und der Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBox1Empty‑Symbol und der angegebenen Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


* Erstellt ein neues Notiz-Tag mit dem BlueCheckBox2Empty‑Symbol und der Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBox2Empty‑Symbol und der angegebenen Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


* Erstellt ein neues Notiz-Tag mit dem BlueCheckBox3Empty‑Symbol und der Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueCheckBox3Empty‑Symbol und der angegebenen Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


* Erstellt ein neues Notiz-Tag mit dem BlueExclamationCheckBoxEmpty‑Symbol und der Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueExclamationCheckBoxEmpty‑Symbol und der angegebenen Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


* Erstellt ein neues Notiz-Tag mit dem BlueFlagCheckBoxEmpty‑Symbol und der Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit dem BlueFlagCheckBoxEmpty‑Symbol und der angegebenen Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


* Erstellt ein neues Notiz-Tag mit BluePersonCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit BluePersonCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


* Erstellt ein neues Notiz-Tag mit BlueRightArrowCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit BlueRightArrowCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


* Erstellt ein neues Notiz-Tag mit BlueStarCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit BlueStarCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


* Erstellt ein neues Notiz-Tag mit GreenCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


* Erstellt ein neues Notiz-Tag mit GreenCheckBox1Empty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBox1Empty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


* Erstellt ein neues Notiz-Tag mit GreenCheckBox2Empty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBox2Empty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


* Erstellt ein neues Notiz-Tag mit GreenCheckBox3Empty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenCheckBox3Empty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


* Erstellt ein neues Notiz-Tag mit GreenExclamationCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenExclamationCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


* Erstellt ein neues Notiz-Tag mit GreenFlagCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenFlagCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


* Erstellt ein neues Notiz-Tag mit GreenPersonCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenPersonCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


* Erstellt ein neues Notiz-Tag mit GreenRightArrowCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenRightArrowCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


* Erstellt ein neues Notiz-Tag mit GreenStarCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


* Erstellt ein neues Notiz-Kontrollkästchen mit GreenStarCheckBoxEmpty Symbol und angegebener Beschriftung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


* Erstellt ein neues Notiz-Tag mit RedFlagCheckBoxEmpty Symbol und Standardbeschriftung.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit RedFlagCheckBoxEmpty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


\* Erstellt ein neues Notiz‑Tag mit YellowCheckBoxEmpty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBoxEmpty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


\* Erstellt ein neues Notiz‑Tag mit YellowCheckBox1Empty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBox1Empty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


\* Erstellt ein neues Notiz‑Tag mit YellowCheckBox2Empty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBox2Empty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


\* Erstellt ein neues Notiz‑Tag mit YellowCheckBox3Empty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowCheckBox3Empty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


\* Erstellt ein neues Notiz‑Tag mit YellowExclamationCheckBoxEmpty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowExclamationCheckBoxEmpty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


\* Erstellt ein neues Notiz‑Tag mit YellowPersonCheckBoxEmpty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowPersonCheckBoxEmpty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


\* Erstellt ein neues Notiz‑Tag mit YellowRightArrowCheckBoxEmpty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowRightArrowCheckBoxEmpty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


\* Erstellt ein neues Notiz‑Tag mit YellowStarCheckBoxEmpty‑Icon und Standard‑Label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


\* Erstellt ein neues Notiz‑Kontrollkästchen mit YellowStarCheckBoxEmpty‑Icon und angegebenem Label.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Etikett | java.lang.String | Das Etikett des Tags. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | Das Objekt. |

**Returns:**
boolean - Der `boolean`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt. |

**Returns:**
boolean - Der `boolean`.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Liest oder setzt die Schriftfarbe.

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


Liest oder setzt die Hervorhebungsfarbe.

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


Liest oder setzt das Icon.

Wert: Das [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


Liest oder setzt den Label‑Text.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als Hash-Funktion für den Typ.

**Returns:**
int - Der `int`.
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Liest oder setzt die Schriftfarbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


Liest oder setzt die Hervorhebungsfarbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


Liest oder setzt den Label‑Text.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

