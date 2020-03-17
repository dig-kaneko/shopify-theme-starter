# shopify-theme-starter
:sunflower::rose: shopify-theme-starter :sunflower: :rose:

## TL;DR  
shopifyのテーマ管理をローカルで行うスターターキット  

## セットアップ  

shopifyのthemekitをインストールしていない場合、インストールすること:octopus:     
`brew tap shopify/shopify`  
`brew install themekit`  

## 注意点  
.envファイルはgit ignoreしてあるため、cloneした後各自設定を行いましょう。  

## 開発コマンド  

`theme_watch`: ローカルのテンプレートを監視し、リアルタイムにサーバーへアップする  
（この際、複数人が同じテーマIDで操作すると上書きされるため各自推奨）  
`theme_open`: ローカルのプレビューを立ち上げる  
`theme_download`: live環境のデータをダウンロードし、ローカル環境を上書きする  


## Shopify Command
`theme get --list -p={password} -s={store}`  
接続しているストアのテーマリストを表示、ここのIDを.envのTHEME_IDに設定する。  
  
`theme new --list -p={password} -s={store} -n={テーマ名}`  
新しくテーマを作成する。  
:fire: `config.ymlが上書きされるので元に戻すこと。` :fire:

## ToDo  
Shopify初心者なのでPR募集:sunglasses:  
* [ ] css,jsのアセット管理（Typescript, scss）  
