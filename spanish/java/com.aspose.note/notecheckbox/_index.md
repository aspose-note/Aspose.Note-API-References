---
title: "NoteCheckBox"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa una etiqueta de nota que puede alternar su estado entre completa e incompleta."
type: docs
weight: 53
url: /es/java/com.aspose.note/notecheckbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)

**All Implemented Interfaces:**
[com.aspose.note.INoteTag](../../com.aspose.note/inotetag), com.aspose.ms.System.IEquatable
```
public class NoteCheckBox extends CheckBox implements INoteTag, System.IEquatable<NoteCheckBox>
```

Representa una etiqueta de nota que puede alternar su estado entre completa e incompleta.
## Métodos

| Método | Descripción |
| --- | --- |
| [createBlueCheckBox()](#createBlueCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono BlueCheckBoxEmpty y la etiqueta predeterminada. |
| [createBlueCheckBox(String label)](#createBlueCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBoxEmpty y la etiqueta especificada. |
| [createBlueCheckBox1()](#createBlueCheckBox1--) | \* Crea una nueva etiqueta de nota con el ícono BlueCheckBox1Empty y la etiqueta predeterminada. |
| [createBlueCheckBox1(String label)](#createBlueCheckBox1-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBox1Empty y la etiqueta especificada. |
| [createBlueCheckBox2()](#createBlueCheckBox2--) | \* Crea una nueva etiqueta de nota con el ícono BlueCheckBox2Empty y la etiqueta predeterminada. |
| [createBlueCheckBox2(String label)](#createBlueCheckBox2-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBox2Empty y la etiqueta especificada. |
| [createBlueCheckBox3()](#createBlueCheckBox3--) | \* Crea una nueva etiqueta de nota con el ícono BlueCheckBox3Empty y la etiqueta predeterminada. |
| [createBlueCheckBox3(String label)](#createBlueCheckBox3-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBox3Empty y la etiqueta especificada. |
| [createBlueExclamationCheckBox()](#createBlueExclamationCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono BlueExclamationCheckBoxEmpty y la etiqueta predeterminada. |
| [createBlueExclamationCheckBox(String label)](#createBlueExclamationCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono BlueExclamationCheckBoxEmpty y la etiqueta especificada. |
| [createBlueFlagCheckBox()](#createBlueFlagCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono BlueFlagCheckBoxEmpty y la etiqueta predeterminada. |
| [createBlueFlagCheckBox(String label)](#createBlueFlagCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono BlueFlagCheckBoxEmpty y la etiqueta especificada. |
| [createBluePersonCheckBox()](#createBluePersonCheckBox--) | * Crea una nueva etiqueta de nota con el ícono BluePersonCheckBoxEmpty y la etiqueta predeterminada. |
| [createBluePersonCheckBox(String label)](#createBluePersonCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono BluePersonCheckBoxEmpty y la etiqueta especificada. |
| [createBlueRightArrowCheckBox()](#createBlueRightArrowCheckBox--) | * Crea una nueva etiqueta de nota con el ícono BlueRightArrowCheckBoxEmpty y la etiqueta predeterminada. |
| [createBlueRightArrowCheckBox(String label)](#createBlueRightArrowCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono BlueRightArrowCheckBoxEmpty y la etiqueta especificada. |
| [createBlueStarCheckBox()](#createBlueStarCheckBox--) | * Crea una nueva etiqueta de nota con el ícono BlueStarCheckBoxEmpty y la etiqueta predeterminada. |
| [createBlueStarCheckBox(String label)](#createBlueStarCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono BlueStarCheckBoxEmpty y la etiqueta especificada. |
| [createGreenCheckBox()](#createGreenCheckBox--) | * Crea una nueva etiqueta de nota con el ícono GreenCheckBoxEmpty y la etiqueta predeterminada. |
| [createGreenCheckBox(String label)](#createGreenCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenCheckBoxEmpty y la etiqueta especificada. |
| [createGreenCheckBox1()](#createGreenCheckBox1--) | * Crea una nueva etiqueta de nota con el ícono GreenCheckBox1Empty y la etiqueta predeterminada. |
| [createGreenCheckBox1(String label)](#createGreenCheckBox1-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenCheckBox1Empty y la etiqueta especificada. |
| [createGreenCheckBox2()](#createGreenCheckBox2--) | * Crea una nueva etiqueta de nota con el ícono GreenCheckBox2Empty y la etiqueta predeterminada. |
| [createGreenCheckBox2(String label)](#createGreenCheckBox2-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenCheckBox2Empty y la etiqueta especificada. |
| [createGreenCheckBox3()](#createGreenCheckBox3--) | * Crea una nueva etiqueta de nota con el ícono GreenCheckBox3Empty y la etiqueta predeterminada. |
| [createGreenCheckBox3(String label)](#createGreenCheckBox3-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenCheckBox3Empty y la etiqueta especificada. |
| [createGreenExclamationCheckBox()](#createGreenExclamationCheckBox--) | * Crea una nueva etiqueta de nota con el ícono GreenExclamationCheckBoxEmpty y la etiqueta predeterminada. |
| [createGreenExclamationCheckBox(String label)](#createGreenExclamationCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenExclamationCheckBoxEmpty y la etiqueta especificada. |
| [createGreenFlagCheckBox()](#createGreenFlagCheckBox--) | * Crea una nueva etiqueta de nota con el ícono GreenFlagCheckBoxEmpty y la etiqueta predeterminada. |
| [createGreenFlagCheckBox(String label)](#createGreenFlagCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenFlagCheckBoxEmpty y la etiqueta especificada. |
| [createGreenPersonCheckBox()](#createGreenPersonCheckBox--) | * Crea una nueva etiqueta de nota con el ícono GreenPersonCheckBoxEmpty y la etiqueta predeterminada. |
| [createGreenPersonCheckBox(String label)](#createGreenPersonCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenPersonCheckBoxEmpty y la etiqueta especificada. |
| [createGreenRightArrowCheckBox()](#createGreenRightArrowCheckBox--) | * Crea una nueva etiqueta de nota con el ícono GreenRightArrowCheckBoxEmpty y la etiqueta predeterminada. |
| [createGreenRightArrowCheckBox(String label)](#createGreenRightArrowCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenRightArrowCheckBoxEmpty y la etiqueta especificada. |
| [createGreenStarCheckBox()](#createGreenStarCheckBox--) | * Crea una nueva etiqueta de nota con el ícono GreenStarCheckBoxEmpty y la etiqueta predeterminada. |
| [createGreenStarCheckBox(String label)](#createGreenStarCheckBox-java.lang.String-) | * Crea una nueva casilla de verificación de nota con el ícono GreenStarCheckBoxEmpty y la etiqueta especificada. |
| [createRedFlagCheckBox()](#createRedFlagCheckBox--) | * Crea una nueva etiqueta de nota con el ícono RedFlagCheckBoxEmpty y la etiqueta predeterminada. |
| [createRedFlagCheckBox(String label)](#createRedFlagCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono RedFlagCheckBoxEmpty y la etiqueta especificada. |
| [createYellowCheckBox()](#createYellowCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono YellowCheckBoxEmpty y la etiqueta predeterminada. |
| [createYellowCheckBox(String label)](#createYellowCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBoxEmpty y la etiqueta especificada. |
| [createYellowCheckBox1()](#createYellowCheckBox1--) | \* Crea una nueva etiqueta de nota con el ícono YellowCheckBox1Empty y la etiqueta predeterminada. |
| [createYellowCheckBox1(String label)](#createYellowCheckBox1-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBox1Empty y la etiqueta especificada. |
| [createYellowCheckBox2()](#createYellowCheckBox2--) | \* Crea una nueva etiqueta de nota con el ícono YellowCheckBox2Empty y la etiqueta predeterminada. |
| [createYellowCheckBox2(String label)](#createYellowCheckBox2-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBox2Empty y la etiqueta especificada. |
| [createYellowCheckBox3()](#createYellowCheckBox3--) | \* Crea una nueva etiqueta de nota con el ícono YellowCheckBox3Empty y la etiqueta predeterminada. |
| [createYellowCheckBox3(String label)](#createYellowCheckBox3-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBox3Empty y la etiqueta especificada. |
| [createYellowExclamationCheckBox()](#createYellowExclamationCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono YellowExclamationCheckBoxEmpty y la etiqueta predeterminada. |
| [createYellowExclamationCheckBox(String label)](#createYellowExclamationCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowExclamationCheckBoxEmpty y la etiqueta especificada. |
| [createYellowPersonCheckBox()](#createYellowPersonCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono YellowPersonCheckBoxEmpty y la etiqueta predeterminada. |
| [createYellowPersonCheckBox(String label)](#createYellowPersonCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowPersonCheckBoxEmpty y la etiqueta especificada. |
| [createYellowRightArrowCheckBox()](#createYellowRightArrowCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono YellowRightArrowCheckBoxEmpty y la etiqueta predeterminada. |
| [createYellowRightArrowCheckBox(String label)](#createYellowRightArrowCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowRightArrowCheckBoxEmpty y la etiqueta especificada. |
| [createYellowStarCheckBox()](#createYellowStarCheckBox--) | \* Crea una nueva etiqueta de nota con el ícono YellowStarCheckBoxEmpty y la etiqueta predeterminada. |
| [createYellowStarCheckBox(String label)](#createYellowStarCheckBox-java.lang.String-) | \* Crea una nueva casilla de verificación de nota con el ícono YellowStarCheckBoxEmpty y la etiqueta especificada. |
| [equals(NoteCheckBox other)](#equals-com.aspose.note.NoteCheckBox-) | Determina si el objeto especificado es igual al objeto actual. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si el objeto especificado es igual al objeto actual. |
| [getFontColor()](#getFontColor--) | Obtiene o establece el color de la fuente. |
| [getHighlight()](#getHighlight--) | Obtiene o establece el color de resaltado. |
| [getIcon()](#getIcon--) | Obtiene o establece el ícono. |
| [getLabel()](#getLabel--) | Obtiene o establece el texto de la etiqueta. |
| [hashCode()](#hashCode--) | Funciona como una función hash para el tipo. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Obtiene o establece el color de la fuente. |
| [setHighlight(Color value)](#setHighlight-java.awt.Color-) | Obtiene o establece el color de resaltado. |
| [setLabel(String value)](#setLabel-java.lang.String-) | Obtiene o establece el texto de la etiqueta. |
### createBlueCheckBox() {#createBlueCheckBox--}
```
public static NoteCheckBox createBlueCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono BlueCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox(String label) {#createBlueCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1() {#createBlueCheckBox1--}
```
public static NoteCheckBox createBlueCheckBox1()
```


\* Crea una nueva etiqueta de nota con el ícono BlueCheckBox1Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox1(String label) {#createBlueCheckBox1-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox1(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBox1Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2() {#createBlueCheckBox2--}
```
public static NoteCheckBox createBlueCheckBox2()
```


\* Crea una nueva etiqueta de nota con el ícono BlueCheckBox2Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox2(String label) {#createBlueCheckBox2-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox2(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBox2Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3() {#createBlueCheckBox3--}
```
public static NoteCheckBox createBlueCheckBox3()
```


\* Crea una nueva etiqueta de nota con el ícono BlueCheckBox3Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueCheckBox3(String label) {#createBlueCheckBox3-java.lang.String-}
```
public static NoteCheckBox createBlueCheckBox3(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono BlueCheckBox3Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox() {#createBlueExclamationCheckBox--}
```
public static NoteCheckBox createBlueExclamationCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono BlueExclamationCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueExclamationCheckBox(String label) {#createBlueExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueExclamationCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono BlueExclamationCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox() {#createBlueFlagCheckBox--}
```
public static NoteCheckBox createBlueFlagCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono BlueFlagCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueFlagCheckBox(String label) {#createBlueFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueFlagCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono BlueFlagCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox() {#createBluePersonCheckBox--}
```
public static NoteCheckBox createBluePersonCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono BluePersonCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBluePersonCheckBox(String label) {#createBluePersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createBluePersonCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono BluePersonCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox() {#createBlueRightArrowCheckBox--}
```
public static NoteCheckBox createBlueRightArrowCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono BlueRightArrowCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueRightArrowCheckBox(String label) {#createBlueRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueRightArrowCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono BlueRightArrowCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox() {#createBlueStarCheckBox--}
```
public static NoteCheckBox createBlueStarCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono BlueStarCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createBlueStarCheckBox(String label) {#createBlueStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createBlueStarCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono BlueStarCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox() {#createGreenCheckBox--}
```
public static NoteCheckBox createGreenCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono GreenCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox(String label) {#createGreenCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1() {#createGreenCheckBox1--}
```
public static NoteCheckBox createGreenCheckBox1()
```


* Crea una nueva etiqueta de nota con el ícono GreenCheckBox1Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox1(String label) {#createGreenCheckBox1-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox1(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenCheckBox1Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2() {#createGreenCheckBox2--}
```
public static NoteCheckBox createGreenCheckBox2()
```


* Crea una nueva etiqueta de nota con el ícono GreenCheckBox2Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox2(String label) {#createGreenCheckBox2-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox2(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenCheckBox2Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3() {#createGreenCheckBox3--}
```
public static NoteCheckBox createGreenCheckBox3()
```


* Crea una nueva etiqueta de nota con el ícono GreenCheckBox3Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenCheckBox3(String label) {#createGreenCheckBox3-java.lang.String-}
```
public static NoteCheckBox createGreenCheckBox3(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenCheckBox3Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox() {#createGreenExclamationCheckBox--}
```
public static NoteCheckBox createGreenExclamationCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono GreenExclamationCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenExclamationCheckBox(String label) {#createGreenExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenExclamationCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenExclamationCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox() {#createGreenFlagCheckBox--}
```
public static NoteCheckBox createGreenFlagCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono GreenFlagCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenFlagCheckBox(String label) {#createGreenFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenFlagCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenFlagCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox() {#createGreenPersonCheckBox--}
```
public static NoteCheckBox createGreenPersonCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono GreenPersonCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenPersonCheckBox(String label) {#createGreenPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenPersonCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenPersonCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox() {#createGreenRightArrowCheckBox--}
```
public static NoteCheckBox createGreenRightArrowCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono GreenRightArrowCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenRightArrowCheckBox(String label) {#createGreenRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenRightArrowCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenRightArrowCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox() {#createGreenStarCheckBox--}
```
public static NoteCheckBox createGreenStarCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono GreenStarCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createGreenStarCheckBox(String label) {#createGreenStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createGreenStarCheckBox(String label)
```


* Crea una nueva casilla de verificación de nota con el ícono GreenStarCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox() {#createRedFlagCheckBox--}
```
public static NoteCheckBox createRedFlagCheckBox()
```


* Crea una nueva etiqueta de nota con el ícono RedFlagCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createRedFlagCheckBox(String label) {#createRedFlagCheckBox-java.lang.String-}
```
public static NoteCheckBox createRedFlagCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono RedFlagCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox() {#createYellowCheckBox--}
```
public static NoteCheckBox createYellowCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono YellowCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox(String label) {#createYellowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1() {#createYellowCheckBox1--}
```
public static NoteCheckBox createYellowCheckBox1()
```


\* Crea una nueva etiqueta de nota con el ícono YellowCheckBox1Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox1(String label) {#createYellowCheckBox1-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox1(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBox1Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2() {#createYellowCheckBox2--}
```
public static NoteCheckBox createYellowCheckBox2()
```


\* Crea una nueva etiqueta de nota con el ícono YellowCheckBox2Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox2(String label) {#createYellowCheckBox2-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox2(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBox2Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3() {#createYellowCheckBox3--}
```
public static NoteCheckBox createYellowCheckBox3()
```


\* Crea una nueva etiqueta de nota con el ícono YellowCheckBox3Empty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowCheckBox3(String label) {#createYellowCheckBox3-java.lang.String-}
```
public static NoteCheckBox createYellowCheckBox3(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowCheckBox3Empty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox() {#createYellowExclamationCheckBox--}
```
public static NoteCheckBox createYellowExclamationCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono YellowExclamationCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowExclamationCheckBox(String label) {#createYellowExclamationCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowExclamationCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowExclamationCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox() {#createYellowPersonCheckBox--}
```
public static NoteCheckBox createYellowPersonCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono YellowPersonCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowPersonCheckBox(String label) {#createYellowPersonCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowPersonCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowPersonCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox() {#createYellowRightArrowCheckBox--}
```
public static NoteCheckBox createYellowRightArrowCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono YellowRightArrowCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowRightArrowCheckBox(String label) {#createYellowRightArrowCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowRightArrowCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowRightArrowCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox() {#createYellowStarCheckBox--}
```
public static NoteCheckBox createYellowStarCheckBox()
```


\* Crea una nueva etiqueta de nota con el ícono YellowStarCheckBoxEmpty y la etiqueta predeterminada.

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### createYellowStarCheckBox(String label) {#createYellowStarCheckBox-java.lang.String-}
```
public static NoteCheckBox createYellowStarCheckBox(String label)
```


\* Crea una nueva casilla de verificación de nota con el ícono YellowStarCheckBoxEmpty y la etiqueta especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| label | java.lang.String | La etiqueta de la etiqueta. |

**Returns:**
[NoteCheckBox](../../com.aspose.note/notecheckbox) - The [NoteCheckBox](../../com.aspose.note/notecheckbox).
### equals(NoteCheckBox other) {#equals-com.aspose.note.NoteCheckBox-}
```
public final boolean equals(NoteCheckBox other)
```


Determina si el objeto especificado es igual al objeto actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [NoteCheckBox](../../com.aspose.note/notecheckbox) | El objeto. |

**Returns:**
boolean - El `boolean`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si el objeto especificado es igual al objeto actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto. |

**Returns:**
boolean - El `boolean`.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Obtiene o establece el color de la fuente.

**Returns:**
java.awt.Color
### getHighlight() {#getHighlight--}
```
public final Color getHighlight()
```


Obtiene o establece el color de resaltado.

**Returns:**
java.awt.Color
### getIcon() {#getIcon--}
```
public int getIcon()
```


Obtiene o establece el ícono.

Valor: El [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public final String getLabel()
```


Obtiene o establece el texto de la etiqueta.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funciona como una función hash para el tipo.

**Returns:**
int - El `int`.
### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Obtiene o establece el color de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color |  |

### setHighlight(Color value) {#setHighlight-java.awt.Color-}
```
public final void setHighlight(Color value)
```


Obtiene o establece el color de resaltado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color |  |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


Obtiene o establece el texto de la etiqueta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

