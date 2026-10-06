# 第2回 Webエンジニアリング演習 レポート
## 学籍番号
4724107
## コンフリクトが発生した理由
（2つのブランチと同じ行の変更を説明）
別の作業ブランチで同じ行に別々の文を加えたため。
## 解決手順
README内のどちらか残したい方の文章以外を削除し、$ git add README.md　$ git commit -m "Resolve README conflict"　$ git pushを順に行って保存すればコンフリクトは解消される。
（実行した操作を順に記載）
## 履歴
（git log --oneline --graph --all の結果）
*   53a7626 (HEAD -> practice/conflict-b, origin/practice/conflict-b) Resolve README conflict
|\  
| *   7981de6 (origin/main, origin/HEAD) Merge pull request #2 from 4724107/practice/conflict-a
| |\  
| | * bfd567a (origin/practice/conflict-a, practice/conflict-a) update goal in conflict A
| |/  
* / 95d9ef0 Update goal in conflict B
|/  
*   47833f3 (main) Merge pull request #1 from 4724107/feature/add-readme
|\  
| * 1bfa93e (origin/feature/add-readme) Add README
|/  
* 9ae7eb2 Add REPORT_01.md
* f79637a Add index.html
* ed6426b Create devcontainer.json
* 802f59b Initial commit