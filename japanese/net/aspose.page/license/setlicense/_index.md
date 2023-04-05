---
title: License.SetLicense
second_title: Aspose.Page for .NET API リファレンス
description: License 方法. コンポーネントのライセンスを取得します
type: docs
weight: 30
url: /ja/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

コンポーネントのライセンスを取得します。

```csharp
public void SetLicense(string licenseName)
```

### 備考

次の場所でライセンスを見つけようとします。

1. 明示的なパス。

2. コンポーネント アセンブリのフォルダ。

3. クライアントの呼び出しアセンブリのフォルダー。

4. エントリ アセンブリのフォルダ。

5. クライアントの呼び出しアセンブリに埋め込まれたリソース。

**ノート：**.NET Compact Framework では、次の場所でのみライセンスを見つけようとします。

1. 明示的なパス。

2. クライアントの呼び出しアセンブリに埋め込まれたリソース。

2. コンポーネント jar ファイルのフォルダー。

### 例

この例では、 を含むフォルダーで MyLicense.lic という名前のライセンス ファイルを検索しようとします。 呼び出しアセンブリを含むフォルダー内のコンポーネント、 エントリ アセンブリのフォルダー内、および呼び出しアセンブリの埋め込みリソース内のコンポーネント.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

コンポーネント jar ファイル:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

完全または短いファイル名にすることができますまたは埋め込みリソースの名前. 空の文字列を使用して、評価モードに切り替えます。

### 関連項目

* class [License](../)
* 名前空間 [Aspose.Page](../../license/)
* 組み立て [Aspose.Page](../../../)

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

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### 関連項目

* class [License](../)
* 名前空間 [Aspose.Page](../../license/)
* 組み立て [Aspose.Page](../../../)


