# ctrl-ime-ahk

## 概要

左右 Ctrl キーの空打ちで IME を OFF/ON する AutoHotKey スクリプトです。

* 左 Ctrl キーの空打ちで IME を「英数」に切り替え
* 右 Ctrl キーの空打ちで IME を「かな」に切り替え
* Ctrl キーを押している間に他のキーを打つと通常の Ctrl キーとして動作（Ctrl+C, Ctrl+V等のショートカットは正常動作）

## 動作環境

* Windows10

## 使い方

最新リリースから ctrl-ime-ahk.exe をダウンロードして好きな場所に置き、起動してください。タスクトレイに常駐します。

**ダウンロード:** [ctrl-ime-ahk v1.0.0](https://github.com/AugusTaro/ctrl-ime-ahk/releases/download/1.0.0/ctrl-ime-ahk.exe) から ctrl-ime-ahk.exe をダウンロードしてください。

### 自分でコンパイルする場合

**前提条件**: AutoHotkey v1.1系がインストールされている必要があります。

**コンパイル方法:**
```bash
"C:\Program Files\AutoHotkey\Compiler\Ahk2Exe.exe" /in "ctrl-ime-ahk.ahk" /out "ctrl-ime-ahk.exe"
```

または、AutoHotkey Compiler (Ahk2Exe.exe) のGUIから：
1. Source (script file): `ctrl-ime-ahk.ahk` を選択
2. Destination (.exe file): `ctrl-ime-ahk.exe` を指定
3. Convert をクリック

終了する場合はタスクトレイのアイコンを右クリックし、「終了」をクリックしてください。

アンインストールは ctrl-ime-ahk.exe を削除するだけで OK です。

## JetBrains 製の IDE で使う場合は Tool Buttons をオンに

IntelliJ IDEA など JetBrains 製の IDE をお使いの方は「上部メニューバー　＞　View　＞　Tool Buttons」をオンにしてください。

オフのまま使うと Ctrl キーを離した際に ctrl-ime-ahk.exe がエラー終了する可能性があります。

## 元プロジェクト

このプロジェクトは [alt-ime-ahk](https://github.com/karakaram/alt-ime-ahk) をベースに、AltキーからCtrlキーに変更したバージョンです。

[Altの空打ちで日本語入力(IME)を切り替えるツールを作った](http://www.karakaram.com/alt-ime-on-off/)

