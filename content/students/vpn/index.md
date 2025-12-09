---
title: "学科VPNの使い方"
---
## VPNでできること

コース内でのみアクセスができるサイトなどに学外からアクセスできます。

---
## MacOSの場合
#### FortiClientをダウンロード
>現在のFortiClientのバージョン(7.4)では起動時にクラッシュするバグが発生しています。
旧バージョンの7.0を[ここからダウンロード](https://filestore.fortinet.com/forticlient/downloads/FortiClientVPNOnlineInstaller_7.0.dmg)
してください

ダウンロードできたらdmgファイルを開きましょう
![This is a image](images/mac1.png)

「FortiClientUpdate.app」を開き警告の「開く」をクリック
![This is a image](images/mac2.png)

しばらく待ち、Installをクリック
![This is a image](images/mac3.png)

続けるをクリックしてください
![This is a image](images/mac4.png)

続けるをクリックしてください
![This is a image](images/mac5.png)

同意するをクリックしてください
![This is a image](images/mac6.png)

続けるをクリックしてください
![This is a image](images/mac7.png)

インストールをクリックしてください
![This is a image](images/mac8.png)

パソコンの認証をしてください
![This is a image](images/mac9.png)

VPNの恒星の追加を求められたら「許可」を押してください
![This is a image](images/mac10.png)

インストーラーはゴミ箱に入れましょう  
![This is a image](images/mac11.png)![This is a image](images/mac12.png)


### FortiClientの設定

VPNに接続するには、FortiClientを使う必要があります。

FortiClientを開いてチェックボックスをクリックし、Iacceptをクリックします。
![This is a image](images/mac_s1.png)

VPN設定をクリック
既存のVPN設定がある場合、VPN名称の右側にある三本線をクリックし、`新規接続の追加`からお願いします。
![This is a image](images/mac_s2.png)


- VPNは、真ん中の`IPsec VPN`を選んでください。
- 
接続名、説明は任意の文字を入れましょう。以下ではわかりやすく`ie-IPsecVPN`にしています。
- リモートGWは`133.13.48.254`を入力してください。 
- 
認証方法は、事前共有鍵を選択し、下の枠には、`nah6gahGicooNaiy`を入力してください。※この事前共有鍵は、外部と共有しないようにしてください。
- ユーザー名は自分の学科アカウント名を入力してください。  
- 最後に保存してください。
![This is a image](images/mac_s3.png)

学科アカウントのパスワードを入力してVPNに接続してください。
![This is a image](images/mac_s4.png)

警告が出た場合は、「続ける」を選択してください。
![This is a image](images/mac_ss.png)

以下のような画面になったら成功です。
![This is a image](images/mac_s5.png)


## Windowsの場合
### FortiClientをダウンロード
>現在のFortiClientのバージョン(7.4)では起動時にクラッシュするバグが発生しています。
旧バージョンの7.0を[ここからダウンロード](https://filestore.fortinet.com/forticlient/downloads/FortiClientVPNOnlineInstaller_7.0.exe)
してください

インストーラーを実行してしばらく待ちましょう
![This is a image](images/win1.png)

- [ ] Yes, I have read and accept
にチェックを入れてNextをクリック
![This is a image](images/win2.png)

インストールを終えて追加されていることを確認
![This is a image](images/win3.png)

### FortiClientの設定
FortiClientを開いてVPN設定をクリック
既存のVPN設定がある場合、VPN名称の右側にある三本線をクリックし、`新規接続の追加`からお願いします。
![This is a image](images/win4.png)


- VPNは、真ん中の`IPsec VPN`を選んでください。
- 
接続名、説明は任意の文字を入れましょう。以下ではわかりやすく`ie-IPsecVPN`にしています。
- リモートGWは`133.13.48.254`を入力してください。 
- 
認証方法は、事前共有鍵を選択し、下の枠には、`nah6gahGicooNaiy`を入力してください。※この事前共有鍵は、外部と共有しないようにしてください。
- ユーザー名は自分の学科アカウント名(例: e235702)を入力してください。  
- 最後に保存してください。。
![This is a image](images/win5.png)

学科アカウントのパスワードを入力すると接続できます
![This is a image](images/win6.png)

もしセキュリティの警告が出た場合[はい]を選択
![This is a image](images/win7.png)

接続に成功すると以下のような画面が表示されます。
![This is a image](images/win8.png)

---
番外編
## sshuttleでアクセス
amane経由で学科サービスにアクセスする方法(sshの設定が必要)

`sshuttle --dns -NHr amane アクセスしたいURL`


