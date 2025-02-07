<h1><img src="./aiscript.svg" alt="AiScript" width="300"></h1>

[![](https://img.shields.io/npm/v/@syuilo/aiscript.svg?style=flat-square)](https://www.npmjs.com/package/@syuilo/aiscript)
[![Test](https://github.com/syuilo/aiscript/actions/workflows/test.yml/badge.svg)](https://github.com/syuilo/aiscript/actions/workflows/test.yml)
[![codecov](https://codecov.io/gh/syuilo/aiscript/branch/master/graph/badge.svg?token=R6IQZ3QJOL)](https://codecov.io/gh/syuilo/aiscript)
[![](https://img.shields.io/badge/license-MIT-444444.svg?style=flat-square)](http://opensource.org/licenses/MIT)
[![](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square&logo=github)](http://makeapullrequest.com)

> **AiScript** is a lightweight scripting language runing on JavaScript.

[Play online ▶](https://syuilo.github.io/aiscript/)

[Read translated version (en)](./translations/en/README.md)

AiScriptは、JavaScript上で動作する軽量プログラミング言語です。AltJSではありません(1)。

* 配列、オブジェクト、関数等をファーストクラスでサポート
* 条件分岐やブロックも式として扱えるなどの柔軟さ
* セミコロンやカンマは不要で書きやすい
* セキュア(2)なサンドボックス環境で実行される
* ホストから変数や関数を提供可能

> (1) ... JavaScript「上で動作」するのであって、JavaScriptに「変換される」のではありません。したがってAltJSではありません。

> (2) ... ホストの情報にアクセスできないこと。

このリポジトリには、JavaScriptで実装されたパーサーと処理系が含まれます。

Note: AiScript and [Misskey](https://github.com/syuilo/misskey) are completely independent projects. AiScript does not prescribe any specific host, but Misskey is the largest user of AiScript (today!)

## Getting started (language)
[See here](./docs/get-started.md)

## Getting started (host implementation)
todo

## Example programs
### Hello world
```
<: "Hello, world!"
```

### Fizz Buzz
```
for (#i, 100) {
  <: if (i % 15 == 0) "FizzBuzz"
    elif (i % 3 == 0) "Fizz"
    elif (i % 5 == 0) "Buzz"
    else i
}
```

## License
[MIT](LICENSE)
