---
title: NoteCheckBox
second_title: Aspose.Note for Java API Reference
description: Represents a note tag that can toggle their state between complete and incomplete.
type: docs
weight: 53
url: /java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

Represents a note tag that can toggle their state between complete and incomplete.
## Methods

| Method | Description |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | \* Creates a new note tag with BlueCheckBoxEmpty icon and default label. |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | \* Creates a new note checkbox with BlueCheckBoxEmpty icon and specified label. |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | \* Creates a new note tag with BlueCheckBox1Empty icon and default label. |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | \* Creates a new note checkbox with BlueCheckBox1Empty icon and specified label. |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | \* Creates a new note tag with BlueCheckBox2Empty icon and default label. |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | \* Creates a new note checkbox with BlueCheckBox2Empty icon and specified label. |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | \* Creates a new note tag with BlueCheckBox3Empty icon and default label. |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | \* Creates a new note checkbox with BlueCheckBox3Empty icon and specified label. |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | \* Creates a new note tag with BlueExclamationCheckBoxEmpty icon and default label. |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | \* Creates a new note checkbox with BlueExclamationCheckBoxEmpty icon and specified label. |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | \* Creates a new note tag with BlueFlagCheckBoxEmpty icon and default label. |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | \* Creates a new note checkbox with BlueFlagCheckBoxEmpty icon and specified label. |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | \* Creates a new note tag with BluePersonCheckBoxEmpty icon and default label. |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | \* Creates a new note checkbox with BluePersonCheckBoxEmpty icon and specified label. |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | \* Creates a new note tag with BlueRightArrowCheckBoxEmpty icon and default label. |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | \* Creates a new note checkbox with BlueRightArrowCheckBoxEmpty icon and specified label. |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | \* Creates a new note tag with BlueStarCheckBoxEmpty icon and default label. |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | \* Creates a new note checkbox with BlueStarCheckBoxEmpty icon and specified label. |
| [createGreenCheckBox()](#createGreenCheckBox--) | \* Creates a new note tag with GreenCheckBoxEmpty icon and default label. |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | \* Creates a new note checkbox with GreenCheckBoxEmpty icon and specified label. |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | \* Creates a new note tag with GreenCheckBox1Empty icon and default label. |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | \* Creates a new note checkbox with GreenCheckBox1Empty icon and specified label. |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | \* Creates a new note tag with GreenCheckBox2Empty icon and default label. |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | \* Creates a new note checkbox with GreenCheckBox2Empty icon and specified label. |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | \* Creates a new note tag with GreenCheckBox3Empty icon and default label. |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | \* Creates a new note checkbox with GreenCheckBox3Empty icon and specified label. |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | \* Creates a new note tag with GreenExclamationCheckBoxEmpty icon and default label. |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | \* Creates a new note checkbox with GreenExclamationCheckBoxEmpty icon and specified label. |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | \* Creates a new note tag with GreenFlagCheckBoxEmpty icon and default label. |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | \* Creates a new note checkbox with GreenFlagCheckBoxEmpty icon and specified label. |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | \* Creates a new note tag with GreenPersonCheckBoxEmpty icon and default label. |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | \* Creates a new note checkbox with GreenPersonCheckBoxEmpty icon and specified label. |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | \* Creates a new note tag with GreenRightArrowCheckBoxEmpty icon and default label. |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | \* Creates a new note checkbox with GreenRightArrowCheckBoxEmpty icon and specified label. |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | \* Creates a new note tag with GreenStarCheckBoxEmpty icon and default label. |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | \* Creates a new note checkbox with GreenStarCheckBoxEmpty icon and specified label. |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | \* Creates a new note tag with RedFlagCheckBoxEmpty icon and default label. |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | \* Creates a new note checkbox with RedFlagCheckBoxEmpty icon and specified label. |
| [createYellowCheckBox()](#createYellowCheckBox--) | \* Creates a new note tag with YellowCheckBoxEmpty icon and default label. |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | \* Creates a new note checkbox with YellowCheckBoxEmpty icon and specified label. |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | \* Creates a new note tag with YellowCheckBox1Empty icon and default label. |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | \* Creates a new note checkbox with YellowCheckBox1Empty icon and specified label. |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | \* Creates a new note tag with YellowCheckBox2Empty icon and default label. |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | \* Creates a new note checkbox with YellowCheckBox2Empty icon and specified label. |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | \* Creates a new note tag with YellowCheckBox3Empty icon and default label. |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | \* Creates a new note checkbox with YellowCheckBox3Empty icon and specified label. |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | \* Creates a new note tag with YellowExclamationCheckBoxEmpty icon and default label. |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | \* Creates a new note checkbox with YellowExclamationCheckBoxEmpty icon and specified label. |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | \* Creates a new note tag with YellowPersonCheckBoxEmpty icon and default label. |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | \* Creates a new note checkbox with YellowPersonCheckBoxEmpty icon and specified label. |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | \* Creates a new note tag with YellowRightArrowCheckBoxEmpty icon and default label. |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | \* Creates a new note checkbox with YellowRightArrowCheckBoxEmpty icon and specified label. |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | \* Creates a new note tag with YellowStarCheckBoxEmpty icon and default label. |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | \* Creates a new note checkbox with YellowStarCheckBoxEmpty icon and specified label. |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | Determines whether the specified object is equal to the current object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether the specified object is equal to the current object. |
| [getFontColor()](#getFontColor--) | Gets or sets the font color. |
| [getHighlight()](#getHighlight--) | Gets or sets the highlight color. |
| [getIcon()](#getIcon--) | Gets or sets the icon. |
| [getLabel()](#getLabel--) | Gets or sets the label text. |
| [hashCode()](#hashCode--) | Serves as a hash function for the type. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Gets or sets the font color. |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | Gets or sets the highlight color. |
| [setLabel(String value)](#setLabel-java.lang.String-) | Gets or sets the label text. |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


\* Creates a new note tag with BlueCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


\* Creates a new note checkbox with BlueCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


\* Creates a new note tag with BlueCheckBox1Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


\* Creates a new note checkbox with BlueCheckBox1Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


\* Creates a new note tag with BlueCheckBox2Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


\* Creates a new note checkbox with BlueCheckBox2Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


\* Creates a new note tag with BlueCheckBox3Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


\* Creates a new note checkbox with BlueCheckBox3Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


\* Creates a new note tag with BlueExclamationCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


\* Creates a new note checkbox with BlueExclamationCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


\* Creates a new note tag with BlueFlagCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


\* Creates a new note checkbox with BlueFlagCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


\* Creates a new note tag with BluePersonCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


\* Creates a new note checkbox with BluePersonCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


\* Creates a new note tag with BlueRightArrowCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


\* Creates a new note checkbox with BlueRightArrowCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


\* Creates a new note tag with BlueStarCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


\* Creates a new note checkbox with BlueStarCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


\* Creates a new note tag with GreenCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


\* Creates a new note checkbox with GreenCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


\* Creates a new note tag with GreenCheckBox1Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


\* Creates a new note checkbox with GreenCheckBox1Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


\* Creates a new note tag with GreenCheckBox2Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


\* Creates a new note checkbox with GreenCheckBox2Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


\* Creates a new note tag with GreenCheckBox3Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


\* Creates a new note checkbox with GreenCheckBox3Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


\* Creates a new note tag with GreenExclamationCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


\* Creates a new note checkbox with GreenExclamationCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


\* Creates a new note tag with GreenFlagCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


\* Creates a new note checkbox with GreenFlagCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


\* Creates a new note tag with GreenPersonCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


\* Creates a new note checkbox with GreenPersonCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


\* Creates a new note tag with GreenRightArrowCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


\* Creates a new note checkbox with GreenRightArrowCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


\* Creates a new note tag with GreenStarCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


\* Creates a new note checkbox with GreenStarCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


\* Creates a new note tag with RedFlagCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


\* Creates a new note checkbox with RedFlagCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


\* Creates a new note tag with YellowCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


\* Creates a new note checkbox with YellowCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


\* Creates a new note tag with YellowCheckBox1Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


\* Creates a new note checkbox with YellowCheckBox1Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


\* Creates a new note tag with YellowCheckBox2Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


\* Creates a new note checkbox with YellowCheckBox2Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


\* Creates a new note tag with YellowCheckBox3Empty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


\* Creates a new note checkbox with YellowCheckBox3Empty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


\* Creates a new note tag with YellowExclamationCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


\* Creates a new note checkbox with YellowExclamationCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


\* Creates a new note tag with YellowPersonCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


\* Creates a new note checkbox with YellowPersonCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


\* Creates a new note tag with YellowRightArrowCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


\* Creates a new note checkbox with YellowRightArrowCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


\* Creates a new note tag with YellowStarCheckBoxEmpty icon and default label.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


\* Creates a new note checkbox with YellowStarCheckBoxEmpty icon and specified label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| label | java.lang.String | The tag's label. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


Determines whether the specified object is equal to the current object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | The object. |

**Returns:**
boolean - The `boolean`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the specified object is equal to the current object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object. |

**Returns:**
boolean - The `boolean`.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Gets or sets the font color.

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


Gets or sets the highlight color.

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


Gets or sets the icon.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


Gets or sets the label text.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Serves as a hash function for the type.

**Returns:**
int - The `int`.
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Gets or sets the font color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


Gets or sets the highlight color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


Gets or sets the label text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

