---
title: License.SetLicense
second_title: Aspose.Note for .NET API リファレンス
description: License 方法. コンポーネントのライセンスを取得します
type: docs
weight: 20
url: /ja/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

コンポーネントのライセンスを取得します。

```csharp
public void SetLicense(string licenseName)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| licenseName | String | 完全なファイル名または短いファイル名、または埋め込みリソースの名前を指定できます。 評価モードに切り替えるには、空の文字列を使用します。 |

### 備考

次の場所でライセンスを見つけようとします。

1. 明示的なパス。

2. Aspose コンポーネント アセンブリを含むフォルダー。

3. クライアントの呼び出しアセンブリを含むフォルダー。

4. エントリ (スタートアップ) アセンブリを含むフォルダー。

5. クライアントの呼び出しアセンブリに埋め込まれたリソース。

**ノート：**.NET Compact Framework では、次の場所でのみライセンスを見つけようとします。

1. 明示的なパス。

2. クライアントの呼び出しアセンブリに埋め込まれたリソース。

### 例

ファイルから Aspose.Note のライセンスをロードする方法を示します。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

埋め込みファイル リソースから Aspose.Note のライセンスをロードする方法を示します。

```csharp
// License クラスをインスタンス化する
Aspose.Note.License license = new Aspose.Note.License();

// アセンブリに埋め込まれたライセンス ファイルの名前のみを渡します
license.SetLicense("Aspose.Note.lic");
```

### 関連項目

* class [License](../)
* 名前空間 [Aspose.Note](../../license/)
* 組み立て [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

コンポーネントのライセンスを取得します。

```csharp
public void SetLicense(Stream stream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ライセンスを含むストリーム。 |

### 備考

このメソッドを使用して、ストリームからライセンスをロードします。

### 例

ストリームから Aspose.Note のライセンスをロードする方法を示します。

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### 関連項目

* class [License](../)
* 名前空間 [Aspose.Note](../../license/)
* 組み立て [Aspose.Note](../../../)


