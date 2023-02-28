---
title: Metered.SetMeteredKey
second_title: .NET API 참조용 Aspose.Note
description: Metered 방법. 측정된 공개 및 개인 키를 설정합니다.
type: docs
weight: 30
url: /ko/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

측정된 공개 및 개인 키를 설정합니다.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| publicKey | String | 공개 키입니다. |
| privateKey | String | 개인 키입니다. |

### 비고

측정된 라이센스를 구매한 경우 애플리케이션 시작 시 이 API를 호출해야 하며 일반적으로 이 정도면 충분합니다. 그러나 측정된 경우 24시간 동안 소비 데이터를 업로드하지 못하면 라이센스가 평가 상태로 설정됩니다. 이를 방지하기 위해서는 라이선스 상태를 정기적으로 확인해야 합니다. 평가 상태인 경우 이 API를 다시 호출하십시오.

### 예

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

* class [Metered](../)
* 네임스페이스 [Aspose.Note](../../metered/)
* 집회 [Aspose.Note](../../../)


