# Slomap SPA


## 仮想環境実行
.venv/Scripts/Activate.ps1

## 環境構築
FastAPI+Vuetify+Nginx+Dockerのテンプレートを活用
1. コンテナのビルド&起動
```
$ docker compose up -d --build
```

2. 開発環境起動
```
$ docker compose exec front yarn dev
```

3. http://localhost:3000 にアクセス(viteの開発環境へのアクセス)

4. フロント側のビルド
```
docker compose exec front yarn build
```

5. http://localhost:8000 にアクセス(NGINXによる本番環境へのアクセス)

<br>

## ⚪︎**サービス URL**

[Slomap](https://www.google.com)

<br>

## ⚪︎ 開発のきっかけ


## ⚪︎ ユーザーの課題

### ⚪︎ マネージャーサイド

- 

### ⚪︎ スタッフサイド

- 
### ⚪︎ 実際に掲示される A3 のシフト表



<br>

## ⚪︎ 機能一覧


## ⚪︎ER 図


<br>

## ⚪︎ インフラ構成図


<br>

## ⚪︎ 主な使用技術

| Category       | Technology Stack                                     |
| -------------- | ---------------------------------------------------- |
| Frontend       |                                                      |
| Backend        |                                                      |
| Infrastructure | Amazon Web Services                                  |
| Database       | MySQL(8.0)                                           |
| Environment    | Docker(23.0.5), Docker compose                       |
| CI/CD          | GitHub Actions                                       |
| library        |                                                      |
| Gem            |                                                      |
| etc.           | Git, GitHub, nginx                                   |

<br>

## ⚪︎ 工夫した点

<details>
<summary>１. </summary>


</details>

<details>
<summary>２. </summary>


</details>

<details>
<summary>３. </summary>

- 
</details>

<details>
<summary>４. </summary>

- 

</details>

<details>
<summary>５. GitHubActions使用した自動デプロイ</summary>

- ECR にイメージの push、ECS のタスク・サービスの更新を実施して backend 側の自動デプロイ可能にしています。
- frontend 側では S3 に build したファイルをアップロードし、Cloudfront を更新する様にしました。
- 発火のタイミングとしては個人開発なので、develop ブランチのみ作成し main ブランチにマージした際に発火する様にしています。

</details>

<br>

## ⚪︎ 今後の課題及び追加予定機能

<details>
<summary>1. </summary>

- 
</details>

<details>
<summary>2. </summary>

- 
</details>

<details>
<summary>3.</summary>

- 
</details>

<details>


<details>
