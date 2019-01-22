# pico-blog
PHP製のCMS『pico』でブログを構築するセットです。  
サンプルの記事やタグを参考にご利用ください。  

内容の詳細についてはこちらの記事にまとめています。  
[Nonsense J](https://nonsensej.xyz/articles/2019/01/16_pico_blog)

-----

# 使い方

### 初期構築方法
`pico`ディレクトリにて`composer install`を実行し、  
その`pico`ディレクトリをWEBサーバーに配置すると使えます。  

また`pico/config/config.yml` に設定が記載されているので  
基本的にはそのままでも良いですが、サイト名は変更すると思うので  
その場合は`site_title`を変更するようにしてください。  

### 記事の更新方法
記事を追加するには`pico/content/articles/`配下にmdファイルを作成してください。  
タグを追加するには`pico/content/tags/`配下にmdファイルを作成してください。  


mdファイルの中身は配置してあるSampleを参考にしてください。  
※確認後、サンプルは削除してください。  

### 検証方法
ローカルでDockerにて動作確認するためにdocker-compose用のファイルも置いてあります。  
`docker`ディレクトリにて以下コマンドを実行すればコンテナが立ち上がります。  
※Dockerがインストール済みである必要があります  
```
docker-compose up -d
```

コンテナが立ち上がったらブラウザにて http://localhost:11080/ へアクセスするとページが見れます。  

### サイトマップ
サイトマップを自動生成するプラグインが入っています。  
以下のURLへアクセスするとサイトマップを確認できます。  
https://PicoページのURL/sitemap.xml  
