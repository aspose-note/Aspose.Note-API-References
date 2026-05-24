---
title: "Metered"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt Methoden zum Festlegen des gemessenen Schlüssels bereit."
type: docs
weight: 50
url: /de/java/com.aspose.note/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

Stellt Methoden zum Festlegen des gemessenen Schlüssels bereit.

--------------------

&gt; ```
&gt; In diesem Beispiel wird versucht, den öffentlichen und privaten Schlüssel von metered zu setzen
&gt; ``````

  [C#]

Metered metered = new Metered();
metered.SetMeteredKey(\"PublicKey\", \"PrivateKey\");
  [Visual Basic]
Dim metered As Metered = New Metered
metered.SetMeteredKey(\"PublicKey\", \"PrivateKey\")
  
```

the component jar file:

```

Metered metered = new Metered();
metered.setMeteredKey(\"PublicKey\", \"PrivateKey\");
  
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

