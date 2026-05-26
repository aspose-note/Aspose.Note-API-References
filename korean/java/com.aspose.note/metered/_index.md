---
title: "Metered"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "계량 키를 설정하는 메서드를 제공합니다."
type: docs
weight: 50
url: /ko/java/com.aspose.note/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

계량 키를 설정하는 메서드를 제공합니다.

--------------------

&gt; ```
&gt; 이 예제에서는 metered 공개 키와 개인 키를 설정하려고 시도합니다.
&gt; ``````

  [C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
  [Visual Basic]
Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
  
```

the component jar file:

```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
```


## Constructors

| Constructor | Description |
| --- | --- |
| [Metered()](#Metered--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getConsumptionCredit()](#getConsumptionCredit--) | Gets consumption credit. |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Gets consumption file size. |
| [resetMeteredKey()](#resetMeteredKey--) | Removes previously setup license. |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Sets metered public and private keys. |
### Metered() {#Metered--}
```
public Metered()
```


### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Gets consumption credit.

**Returns:**
java.math.BigDecimal - Returns the number of consumed credit points.
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Gets consumption file size.

**Returns:**
java.math.BigDecimal - Returns the number of consumed bytes.
### resetMeteredKey() {#resetMeteredKey--}
```
public final void resetMeteredKey()
```


Removes previously setup license.

### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Sets metered public and private keys.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | The public key. |
| privateKey | java.lang.String | The private key.

--------------------

If you purchase metered license, this API should be called on application startup, normally, this is enough. However, if metered fails to upload consumption data during 24 hours period, the license will be set to evaluation status. To avoid such case, you should regularly check the license status If it is evaluation status, call this API again. |

