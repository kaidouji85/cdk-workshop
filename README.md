# AWS CDK 写経

## はじめに
[AWS CDK チュートリアル](https://intro-to-cdk.workshop.aws) の写経です

## 動かし方
### 1. clone直後にやること
```shell
cd <本リポジトリをcloneした場所>
npm ci
```

### 2. デプロイ
```shell
cdk deploy
# 一定時間経過後、リソースが作られる
# 成功したら、以下のようにAPI GatewayのURLが表示される
# Outputs:
# CdkWorkshopStack.apiEndpoint9349E63C = <API GatewayのURL>
```
## 3. 動作確認
1. ブラウザで以下にアクセス
```url
https://<API GatewayのURL>/I can't stop thinking about stuff and my sleep is terrible
```
2. ブラウザに以下のようなメッセージが表示される。(メッセージは毎回変わる)
```
{"You":"I can't stop thinking about stuff and my sleep is terrible","ELIZA":"You say you can't stop thinking about stuff and my sleep is terrible ?"}
```