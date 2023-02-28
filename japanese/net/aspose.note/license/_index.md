---
title: Class License
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.License クラス. コンポーネントのライセンスを取得する方法を提供します
type: docs
weight: 310
url: /ja/net/aspose.note/license/
---
## License class

コンポーネントのライセンスを取得する方法を提供します。

```csharp
public class License
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [License](license/)() | デフォルトのコンストラクター。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | コンポーネントのライセンスを取得します。 |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | コンポーネントのライセンスを取得します。 |

### 例

ファイルから Aspose.Note のライセンスをロードする方法を示します。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

ストリームから Aspose.Note のライセンスをロードする方法を示します。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

埋め込みファイル リソースから Aspose.Note のライセンスをロードする方法を示します。

```csharp
// License クラスをインスタンス化する
Aspose.Note.License license = new Aspose.Note.License();

// アセンブリに埋め込まれたライセンス ファイルの名前のみを渡します
license.SetLicense("Aspose.Note.lic");
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


