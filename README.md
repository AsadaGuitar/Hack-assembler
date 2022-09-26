# Hack-assembler
<img src="https://img.shields.io/badge/build-passed-red?logo=sbt" /> <img src="https://img.shields.io/badge/test-complete-green" /> <img src="https://img.shields.io/badge/scala-3.1.2-blue?logo=scala" /> <img src="https://img.shields.io/badge/cats core-2.7.0-blue" />
<br><br>
書籍「コンピューターシステムの理論と実装」第６章　実装課題
16bit Hackコンピュータのアセンブラ。

### 使用ライブラリ
+ [cats-core](https://typelevel.org/cats/)<br>
+ [cats-effect](https://typelevel.org/cats-effect/)<br>
+ [scala-parser-combinators](https://github.com/scala/scala-parser-combinators)<br>

## 要件
+ アセンブリコードによるプログラムは「.asm」、バイナリプログラムは「.hack」という拡張子を持つ。
+ バイナリコードのプログラムは各行「0」と「1」のASCII文字が16個並ぶ16bitのHack機械語とする。
+ アセンブリ言語は命令（A命令・C命令）、シンボル、コメントからなる。（空白はパディングされる）

## 例
アセンブリ言語
```assembly
@COUNT
M = 1
```

バイナリコード
```binary
0000010000000000
1110010111111111
```
