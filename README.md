# (Beta) Postman script for API
THIS IS TO BE USED FOR EVALUATION PURPOSE ONLY. WE ARE NOT HOLDING ANY ACCOUNTABILITY AND RESPONSIBILITY AGAINST ANY CASES OF OUTCOMES BY UTILIZING THE SCRIPTS SHOWN IN THIS REPOSITORY 

エクイニクス製品向けに用意されたPostmanのコレクションです。

[Equinix Fabric Portal](https://fabric.equinix.com/)

## 内容
- Token_generator
- VC_lookup
- NE_lookup
- creation_NEtoPort_VC
- creation_NEtoAzure_ExR_VC

## 要件
1. ご自身のPCに[Postman](https://www.postman.com/downloads/)を導入
2. [Equinix Fabric Portal](https://fabric.equinix.com/)の有効なアカウント。 お持ちでない場合はCSM担当者にご連絡下さい
3. [Equinix Developer Platform](https://developer.equinix.com/)の有効なアカウント。 お持ちでない場合はCSM担当者にご連絡下さい
4. **client_id** と **client_secret**を生成する。 [ガイド](https://developer.equinix.com/docs?page=/dev-docs/fabric/overview)を参照下さい
5.  [Github](https://github.com/) のアカウント

## 設定方法
1. [Postman](https://www.postman.com/)の起動
2. Postmanへデータをインポートするためこちらの [ガイド](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-from-github-repositories)を参照のうえ実施
3. ご自身のデータを変数として入力する
   - 画面右上の**Environment quick look**をクリック
     - <sub>Postman</sub>
     - ![env quicklook](https://user-images.githubusercontent.com/109955201/193489769-ee15fbdf-7e55-4c93-9621-3630e2fbcde8.png)
   - APIコールのため[Equinix Developer Platform](https://developer.equinix.com/)で生成した**client_id**と**client_secret**を変数に入力
     - <sub>Equinix developer platform</sub>
     - <img width="656" alt="userinfo" src="https://user-images.githubusercontent.com/109955201/193498978-87897281-25d6-4c3f-bd26-3532dccc2658.png">
     - <sub>Postman</sub>
     - <img width="703" alt="userinfo2" src="https://user-images.githubusercontent.com/109955201/193501814-47b94912-ef0b-4b5c-9e23-b5cbbf3d8700.png">
   - **vc_uuid**と**ned_uuid**や他の変数パラメータを入力

---
## ユースケース

### VC lookup

1. "Token_generator"コレクションでAPI実行し**access_token**を取得
2. "VC_lookup"コレクションでAPI実行
   - <sub>response successful</sub>
   - ![response](https://user-images.githubusercontent.com/109955201/193509583-0e1c055c-2b3e-4141-88d5-4ac91b88fdaf.png)
