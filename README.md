さくらのクラウド スタートアップスクリプト
====

スタートアップスクリプトは、新たにサーバを作成する際、任意の「スタートアップスクリプト」を選択することにより、起動時にそれらを自動的に実行する機能です。
さくらインターネットが提供しているパブリックスタートアップスクリプトを一覧です

詳細は[さくらのクラウドニュース](https://cloud-news.sakura.ad.jp/startup-script/)をご参照ください

# 提供中スタートアップスクリプト一覧

* [アプリケーション](#application)
* [開発ツール・開発環境・ミドルウェア](#development)
* [さくらのクラウド開発ツール・設定支援](#sacloud)
* [システム管理・運用](#admin)

## <a name="application">アプリケーション</a>

| 分類 | 名前 | 説明 |
| --- | --- | :--- |
| CMS | [Drupal for Ubuntu](./publicscript/Drupal%20for%20Ubuntu) | 高機能CMSであるDrupalをインストールします。<br />※Ubuntu 14.04 または 16.04 でのみ動作します |
| CMS | [Drupal for CentOS 7](./publicscript/Drupal%20for%20CentOS7) | 高機能CMSであるDrupalをインストールします。<br />※CentOS 7でのみ動作します |
| CMS | [SHIRASAGI](./publicscript/SHIRASAGI) | Ruby、Ruby on Rails、MongoDBで動作する中・大規模サイト向けCMS「SHIRASAGI」をインストールします。 [公式サイトはこちら](http://www.ss-proj.org/)です。<br />※CentOS7系のみで動作します |
| CMS | [WordPress](./publicscript/WordPress) | yumにより、ApacheとMySQLをインストール・Wordpres向けの設定を自動的に行い、Wordpress最新バージョンをインストールします。<br />サーバ作成後はサーバのIPアドレスにWebブラウザでアクセスするとWordpress初期画面が表示される状態となります。 |
| CMS | [WordPress for KUSANAGI8](./publicscript/WordPress%20for%20KUSANAGI8) | KUSANAGI8 環境に WordPress をセットアップするスクリプトです。<br />本スクリプトの詳細は[マニュアル](https://cloud-news.sakura.ad.jp/wordpress-for-kusanagi8/)を参照ください。 |
| オンラインストレージ | [ownCloud](./publicscript/owncloud) | ownCloudをセットアップするスクリプトです。<br />サーバ作成後はブラウザより「http://サーバIPアドレス/owncloud/」にアクセスすることでownCloudの設定が行えます。<br />※ownCloudのスタートアップスクリプトでインストールされるPHPのバージョンはownCloudの推奨バージョンより低くなっているため、5.3.8以降のバージョンにアップデートすることを推奨します。 |
| ECプラットフォーム | [Magento](./publicscript/Magento) | 越境ECプラットフォームであるMagentoをインストールします。<br />本スクリプトの詳細は[マニュアル](https://cloud-news.sakura.ad.jp/startup-script/magento/)を参照ください。<br />※Ubuntu 16系のみで動作します |
| SNS | [Mastodon](./publicscript/Mastodon) | Twitterライクな投稿ができる分散型ソーシャルネットワーク「Mastodon」のインスタンス（サーバ）をセットアップします。<br />※CentOS7系のみで動作します |
| 科学計算 | [Jupyter Notebook](./publicscript/Jupyter%20Notebook) | データサイエンス環境としてAnacondaとウェブブラウザ上から手軽にプログラムを実行できるJupyter Notebookを一括でセットアップすることの出来るスタートアップスクリプトです。<br />インストール内容の詳細などは[SlideShare](https://www.slideshare.net/sakura_pr/sakura-cloud-startup-script-jupyter-notebook)をご参照ください。<br />※CentOS7系のみで動作します |
| 分析基盤 | [kibana](./publicscript/Kibana) | 分析基盤としてElasticsearchとKibana、ログ収集のFluentdを一括しセットアップすることの出来るスタートアップスクリプトです。<br />インストール内容の詳細などは[SlideShare](https://www.slideshare.net/sakura_pr/sakura-cloudkibanaelasticsearchstartupscript)をご参照ください。<br />※CentOS7系のみで動作します |


## <a name="development">開発ツール・開発環境・ミドルウェア</a>

| 分類 | 名前 | 説明 |
| --- | --- | :--- |
| 開発支援 | [Git Clone](./publicscript/Git%20Clone) | 指定のGitリポジトリをcloneし、指定の実行ファイルを自動的に実行します。<br />拡張子が .yml のものは Ansible Playbook として解釈されます。 |
| メッセージキュー管理 | [RabbitMQ](./publicscript/RabbitMQ) | メッセージキュー管理システムであるRabbitMQをインストールします。 |
| 開発言語・フレームワーク | [LAMP](./publicscript/LAMP) | yumによりApache、MySQL、PHPをインストールし、LAMP構成を作成します。 | 
| 開発言語・フレームワーク | [Node-RED](./publicscript/Node-RED) | ブラウザの操作だけででハードウェア・デバイスを制御できるプログラミング・ツール「Node-RED」をインストールします。<br />※CentOS7系のみで動作します |
| 開発言語・フレームワーク | [Ruby on Rails](./publicscript/Ruby%20on%20Rails) | スクリプト言語RubyのフレームワークであるRuby on Railsをインストールします。 |
| プロジェクト管理 | [Redmine](./publicscript/Redmine) | プロジェクト管理ソフトウェアのRedmineをインストールし、起動時に動作する状態に設定します。 |


## <a name="sacloud">さくらのクラウド開発ツール・設定支援</a>

| 分類 | 名前 | 説明 |
| --- | --- | :--- |
| 設定支援 | [lb-dsr](./publicscript/lb-dsr) | ロードバランス対象のサーバの初期設定を自動化するためのスクリプトです。<br />このスクリプトは、以下のアーカイブでのみ動作します<br />- CentOS 6.X<br />- CentOS 7.X |
| CLI | [Sacloud CLI](./publicscript/Sacloud%20CLI) | さくらのクラウドで提供しているSacloud CLIと、実行環境のnode.jsをインストールします。 |
| CLI | [Terraform for さくらのクラウド](./publicscript/Terraform%20for%20%E3%81%95%E3%81%8F%E3%82%89%E3%81%AE%E3%82%AF%E3%83%A9%E3%82%A6%E3%83%89) | インフラ構築や構成変更をコードで管理する“Infrastructure as Code“を実現するための、オープンソースのコマンドラインツール「Terraform」およびさくらのクラウドを利用するためのプラグインを一括でインストールします。詳細は「[Terraform for さくらのクラウド](https://cloud-news.sakura.ad.jp/startup-script/terraform-for-sakuracloud/)」をご確認ください。<br />※CentOS7系のみで動作します |


## <a name="admin">システム管理・運用</a>

| 分類 | 名前 | 説明 |
| --- | --- | :--- |
| パッケージ管理 | [yum update](./publicscript/yum%20update) | サーバ作成後の初回起動時のみ、コマンド”yum update”を実行します。実行完了後、サーバが再起動されます。<br />※CentOS6系またはScientific Linux6系のみで動作します |
| パッケージ管理 | [apt-get update/upgrade](./publicscript/apt-get%20update_upgrade) | サーバ作成後の初回起動時のみ、コマンド”apt-get update”および”apt-get upgrade”を実行します。実行完了後、サーバが再起動されます。<br />※DebianまたはUbuntuのみで動作します |
| 監視 | [zabbix-server](./publicscript/zabbix-server) | 監視サーバであるzabbix-serverをインストールします。<br />本スクリプトの詳細は[マニュアル](https://cloud-news.sakura.ad.jp/startup-script/zabbix-server/)を参照ください。<br />※CentOS7系のみで動作します | 
| 監視 | [zabbix-agent](./publicscript/zabbix-agent) | zabbix-serverに対応するエージェントzabbix-agentをインストールします。<br />本スクリプトの詳細は[マニュアル](https://cloud-news.sakura.ad.jp/startup-script/zabbix-agent/)を参照ください。<br />※CentOS7系のみで動作します |
| 監視 | [hatohol-server](./publicscript/hatohol-server) | 複数のzabbix-serverを統合管理するhatoholをインストールします。<br />※CentOS7系のみで動作します
| セキュリティ | [Vuls](./publicscript/Vuls) | オープンソースで開発が進められているLinux/FreeBSD向けの脆弱性スキャンツールです。<br />OSだけでなくミドルウェアやプログラム言語のライブラリなどもスキャンに対応しております。<br />また、エージェントレスで実行させることが出来、SSH経由でリモートのサーバのスキャンを行うことも可能です。<br />※CentOS7系のみで動作します |
