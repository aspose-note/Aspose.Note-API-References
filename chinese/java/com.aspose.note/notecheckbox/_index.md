---
title: "NoteCheckBox"
second_title: "Aspose.Note for Java API 参考"
description: "表示可以在完成和未完成状态之间切换的笔记标签。"
type: docs
weight: 53
url: /zh/java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

表示可以在完成和未完成状态之间切换的笔记标签。
## 方法

| 方法 | 描述 |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | * 创建一个带有 BlueCheckBoxEmpty 图标和默认标签的新笔记标签。 |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | * 创建一个带有 BlueCheckBoxEmpty 图标和指定标签的新笔记复选框。 |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | * 创建一个带有 BlueCheckBox1Empty 图标和默认标签的新笔记标签。 |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | * 创建一个带有 BlueCheckBox1Empty 图标和指定标签的新笔记复选框。 |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | * 创建一个带有 BlueCheckBox2Empty 图标和默认标签的新笔记标签。 |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | * 创建一个带有 BlueCheckBox2Empty 图标和指定标签的新笔记复选框。 |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | * 创建一个带有 BlueCheckBox3Empty 图标和默认标签的新笔记标签。 |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | * 创建一个带有 BlueCheckBox3Empty 图标和指定标签的新笔记复选框。 |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | * 创建一个带有 BlueExclamationCheckBoxEmpty 图标和默认标签的新笔记标签。 |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | * 创建一个带有 BlueExclamationCheckBoxEmpty 图标和指定标签的新笔记复选框。 |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | * 创建一个带有 BlueFlagCheckBoxEmpty 图标和默认标签的新笔记标签。 |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | * 创建一个带有 BlueFlagCheckBoxEmpty 图标和指定标签的新笔记复选框。 |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | * 创建一个带有 BluePersonCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | * 创建一个带有 BluePersonCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | * 创建一个带有 BlueRightArrowCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | * 创建一个带有 BlueRightArrowCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | * 创建一个带有 BlueStarCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | * 创建一个带有 BlueStarCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createGreenCheckBox()](#createGreenCheckBox--) | * 创建一个带有 GreenCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | * 创建一个带有 GreenCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | * 创建一个带有 GreenCheckBox1Empty 图标和默认标签的笔记标签。 |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | * 创建一个带有 GreenCheckBox1Empty 图标和指定标签的笔记复选框。 |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | * 创建一个带有 GreenCheckBox2Empty 图标和默认标签的笔记标签。 |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | * 创建一个带有 GreenCheckBox2Empty 图标和指定标签的笔记复选框。 |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | * 创建一个带有 GreenCheckBox3Empty 图标和默认标签的笔记标签。 |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | * 创建一个带有 GreenCheckBox3Empty 图标和指定标签的笔记复选框。 |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | * 创建一个带有 GreenExclamationCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | * 创建一个带有 GreenExclamationCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | * 创建一个带有 GreenFlagCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | * 创建一个带有 GreenFlagCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | * 创建一个带有 GreenPersonCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | * 创建一个带有 GreenPersonCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | * 创建一个带有 GreenRightArrowCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | * 创建一个带有 GreenRightArrowCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | * 创建一个带有 GreenStarCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | * 创建一个带有 GreenStarCheckBoxEmpty 图标和指定标签的笔记复选框。 |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | * 创建一个带有 RedFlagCheckBoxEmpty 图标和默认标签的笔记标签。 |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | * 创建一个新的笔记复选框，使用 RedFlagCheckBoxEmpty 图标和指定的标签。 |
| [createYellowCheckBox()](#createYellowCheckBox--) | * 创建一个新的笔记标签，使用 YellowCheckBoxEmpty 图标和默认标签。 |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowCheckBoxEmpty 图标和指定的标签。 |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | * 创建一个新的笔记标签，使用 YellowCheckBox1Empty 图标和默认标签。 |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowCheckBox1Empty 图标和指定的标签。 |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | * 创建一个新的笔记标签，使用 YellowCheckBox2Empty 图标和默认标签。 |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowCheckBox2Empty 图标和指定的标签。 |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | * 创建一个新的笔记标签，使用 YellowCheckBox3Empty 图标和默认标签。 |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowCheckBox3Empty 图标和指定的标签。 |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | * 创建一个新的笔记标签，使用 YellowExclamationCheckBoxEmpty 图标和默认标签。 |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowExclamationCheckBoxEmpty 图标和指定的标签。 |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | * 创建一个新的笔记标签，使用 YellowPersonCheckBoxEmpty 图标和默认标签。 |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowPersonCheckBoxEmpty 图标和指定的标签。 |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | * 创建一个新的笔记标签，使用 YellowRightArrowCheckBoxEmpty 图标和默认标签。 |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowRightArrowCheckBoxEmpty 图标和指定的标签。 |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | * 创建一个新的笔记标签，使用 YellowStarCheckBoxEmpty 图标和默认标签。 |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | * 创建一个新的笔记复选框，使用 YellowStarCheckBoxEmpty 图标和指定的标签。 |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | 确定指定的对象是否等于当前对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定指定的对象是否等于当前对象。 |
| [getFontColor()](#getFontColor--) | 获取或设置字体颜色。 |
| [getHighlight()](#getHighlight--) | 获取或设置突出显示颜色。 |
| [getIcon()](#getIcon--) | 获取或设置图标。 |
| [getLabel()](#getLabel--) | 获取或设置标签文本。 |
| [hashCode()](#hashCode--) | 作为该类型的哈希函数。 |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | 获取或设置字体颜色。 |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | 获取或设置突出显示颜色。 |
| [setLabel(String value)](#setLabel-java.lang.String-) | 获取或设置标签文本。 |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


* 创建一个带有 BlueCheckBoxEmpty 图标和默认标签的新笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


* 创建一个带有 BlueCheckBoxEmpty 图标和指定标签的新笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


* 创建一个带有 BlueCheckBox1Empty 图标和默认标签的新笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


* 创建一个带有 BlueCheckBox1Empty 图标和指定标签的新笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


* 创建一个带有 BlueCheckBox2Empty 图标和默认标签的新笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


* 创建一个带有 BlueCheckBox2Empty 图标和指定标签的新笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


* 创建一个带有 BlueCheckBox3Empty 图标和默认标签的新笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


* 创建一个带有 BlueCheckBox3Empty 图标和指定标签的新笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


* 创建一个带有 BlueExclamationCheckBoxEmpty 图标和默认标签的新笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


* 创建一个带有 BlueExclamationCheckBoxEmpty 图标和指定标签的新笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


* 创建一个带有 BlueFlagCheckBoxEmpty 图标和默认标签的新笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


* 创建一个带有 BlueFlagCheckBoxEmpty 图标和指定标签的新笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


* 创建一个带有 BluePersonCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


* 创建一个带有 BluePersonCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


* 创建一个带有 BlueRightArrowCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


* 创建一个带有 BlueRightArrowCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


* 创建一个带有 BlueStarCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


* 创建一个带有 BlueStarCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


* 创建一个带有 GreenCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


* 创建一个带有 GreenCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


* 创建一个带有 GreenCheckBox1Empty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


* 创建一个带有 GreenCheckBox1Empty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


* 创建一个带有 GreenCheckBox2Empty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


* 创建一个带有 GreenCheckBox2Empty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


* 创建一个带有 GreenCheckBox3Empty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


* 创建一个带有 GreenCheckBox3Empty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


* 创建一个带有 GreenExclamationCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


* 创建一个带有 GreenExclamationCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


* 创建一个带有 GreenFlagCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


* 创建一个带有 GreenFlagCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


* 创建一个带有 GreenPersonCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


* 创建一个带有 GreenPersonCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


* 创建一个带有 GreenRightArrowCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


* 创建一个带有 GreenRightArrowCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


* 创建一个带有 GreenStarCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


* 创建一个带有 GreenStarCheckBoxEmpty 图标和指定标签的笔记复选框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


* 创建一个带有 RedFlagCheckBoxEmpty 图标和默认标签的笔记标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


* 创建一个新的笔记复选框，使用 RedFlagCheckBoxEmpty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


* 创建一个新的笔记标签，使用 YellowCheckBoxEmpty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


* 创建一个新的笔记复选框，使用 YellowCheckBoxEmpty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


* 创建一个新的笔记标签，使用 YellowCheckBox1Empty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


* 创建一个新的笔记复选框，使用 YellowCheckBox1Empty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


* 创建一个新的笔记标签，使用 YellowCheckBox2Empty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


* 创建一个新的笔记复选框，使用 YellowCheckBox2Empty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


* 创建一个新的笔记标签，使用 YellowCheckBox3Empty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


* 创建一个新的笔记复选框，使用 YellowCheckBox3Empty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


* 创建一个新的笔记标签，使用 YellowExclamationCheckBoxEmpty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


* 创建一个新的笔记复选框，使用 YellowExclamationCheckBoxEmpty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


* 创建一个新的笔记标签，使用 YellowPersonCheckBoxEmpty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


* 创建一个新的笔记复选框，使用 YellowPersonCheckBoxEmpty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


* 创建一个新的笔记标签，使用 YellowRightArrowCheckBoxEmpty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


* 创建一个新的笔记复选框，使用 YellowRightArrowCheckBoxEmpty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


* 创建一个新的笔记标签，使用 YellowStarCheckBoxEmpty 图标和默认标签。

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


* 创建一个新的笔记复选框，使用 YellowStarCheckBoxEmpty 图标和指定的标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String | 标签的标签。 |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | 对象。 |

**Returns:**
boolean - 该 `boolean`。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 对象 | java.lang.Object | 对象。 |

**Returns:**
boolean - 该 `boolean`。
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


获取或设置字体颜色。

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


获取或设置突出显示颜色。

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


获取或设置图标。

值：该 [TagIcon](../../com.aspose.note.infrastructure/tagicon)。

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


获取或设置标签文本。

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为该类型的哈希函数。

**Returns:**
int - 该 `int`。
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


获取或设置字体颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


获取或设置突出显示颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


获取或设置标签文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

