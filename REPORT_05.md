# 第5回 Webエンジニアリング演習 レポート
## 学籍番号
4724107
## TODO配列のコード
（コードまたは確認結果）
const todos = [
  { id: 1, title: "型を復習する", completed: true },
  { id: 2, title: "配列を学ぶ", completed: false },
  { id: 3, title: "レポートを書く", completed: false },
  { id: 4, title: "コードを提出する", completed: false },
];

## TODOを更新した条件
（コードまたは確認結果）
for (const todo of todos){
    if(todo.completed == false){
        todo.completed = true;
    }
}

## 完了件数の更新前後の実行結果
（コードまたは確認結果）
【コード】
const completedBefore = todos.filter((todo) => todo.completed).length;
for (const todo of todos){
    if(todo.completed == false){
        todo.completed = true;
    }
}
const completedAfter = todos.filter((todo) => todo.completed).length;
console.log(`完了件数: 更新前 ${completedBefore}件 -> 更新後 ${completedAfter}件`);
console.log(`更新後のTODOの状態：`);
for (const todo of todos) {
  const status = todo.completed ? "完了" : "未完了";
  console.log(`${todo.id}: ${todo.title} [${status}]`);
}

【確認結果】
完了件数: 更新前 1件 -> 更新後 4件
更新後のTODOの状態：
1: 型を復習する [完了]
2: 配列を学ぶ [完了]
3: レポートを書く [完了]
4: コードを提出する [完了]
