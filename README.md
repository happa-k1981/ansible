# ansibleインストール

## インストール
1. yum-utilsをインストール(yum-config-managerを使うため)
```
yum install yum-utils
```
2. EPEL、remiをインストール
```
yum install epel-release
```
3. ansbleをインストール
```
yum install ansible
```
4. EPEL,remiを無効化
```
yum-config-manager --disable epel
```

### まとめてやりたい場合は以下のコマンド
```
yum -y install yum-utils epel-release && yum -y install ansible && yum-config-manager --disable epel
```

実行方法
1.srcディレクトリごとサーバーにアップ
2.SSHでログインし、srcディレクトリに移動
3.ansible-playbook common.yml
※rootユーザーになっているのが前提