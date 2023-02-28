---
title: Class Metered
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Metered 수업. 측정 키를 설정하는 방법을 제공합니다.
type: docs
weight: 350
url: /ko/net/aspose.note/metered/
---
## Metered class

측정 키를 설정하는 방법을 제공합니다.

```csharp
public class Metered
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Metered](metered/)() | 기본 생성자입니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | 이전에 설정한 라이센스를 제거합니다. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | 측정된 공개 및 개인 키를 설정합니다. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | 소비 크레딧을 가져옵니다. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | 사용 파일 크기를 가져옵니다. |

### 예

이 예에서는 측정된 공용 및 개인 키 를 설정하려고 시도합니다.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

측정된 라이센스를 설정하는 방법을 보여줍니다.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### 또한보십시오

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


