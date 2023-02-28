---
title: Metered.SetMeteredKey
second_title: Справочник по API Aspose.Note для .NET
description: Metered метод. Устанавливает лимитированные открытые и закрытые ключи.
type: docs
weight: 30
url: /ru/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Устанавливает лимитированные открытые и закрытые ключи.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | String | Открытый ключ. |
| privateKey | String | Закрытый ключ. |

### Примечания

Если вы приобрели лицензию с ограниченным доступом, этот API следует вызывать при запуске приложения, обычно этого достаточно. Чтобы избежать такого случая, вы должны регулярно проверять статус лицензии. Если это статус оценки, снова вызовите этот API.

### Примеры

Показывает, как установить лимитную лицензию.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Смотрите также

* class [Metered](../)
* пространство имен [Aspose.Note](../../metered/)
* сборка [Aspose.Note](../../../)


