# 第6回 Webエンジニアリング演習 レポート
## 学籍番号
4724107
## `Todo`型の定義
（コードまたは確認結果）
コード：
export type Todo = {
   id: number;
   title: string;
   completed: boolean;
   dueDate?: string;
};

## 未完了件数を返す関数の引数と戻り値の型
（コードまたは確認結果）
コード：
export async function incompleteTodos(): Promise<number> {
   const currentTodos = await fetchTodos();
   const incompleteTodos = currentTodos.filter(
     (todo) => !todo.completed,
   );
   return incompleteTodos.length;
}

## 未完了件数の実行結果
（コードまたは確認結果）
コード：
const incomplete = await incompleteTodos();
console.log("未完了TODO件数:",incomplete);
確認結果：
未完了TODO件数: 1