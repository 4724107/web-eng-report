# 第4回 Webエンジニアリング演習 レポート
## 学籍番号
4724107
## `const`と`let`の宣言・再代入に使用したコード
（コードまたは確認結果）
const courseName = "Web Engineering";
let retryCount = 1;
courseName = "Other Course"; 
retryCount = 2;

## VSCodeと`pnpm run check`に表示されたエラー番号・メッセージ
（コードまたは確認結果）
エラー番号：error TS2588:
エラーメッセージ： Cannot assign to 'courseName' because it is a constant.


##　修正後の実行結果と`const`・`let`の違いの説明
（コードまたは確認結果）
実行結果：エラー無し。
@4724107 ➜ /workspaces/web-eng-typescript (main) $ pnpm run check
$ tsc --noEmit src/index.ts
@4724107 ➜ /workspaces/web-eng-typescript (main) $ pnpm run start
$ tsx src/index.ts
キーボード 4800 2 true
10560
キーボードを2個購入する
税込合計は10560円である

constとlet`の違い：
constは再代入が禁止されている変数を宣言するもので、宣言後に別の値を代入しようとするとエラーになり実行できないように防止される。再代入が不要の変数はConstを使用する。
letは再代入が可能な変数を宣言するためのもので、宣言後に別の値を代入してもエラーが起きず更新される。


