* Twitterからデータ取得
* MySQLからデータ取得
* GAからデータ取得
* 定期的な取得
* embulk
* 可視化


# fluentdの設定ファイルのチェック

```sh
docker-compose run --rm collector fluentd --dry-run -c /fluentd/etc/fluent.conf
```

fluentdにjsonをポスト

```
http://192.168.99.100:24220/api/plugins?tag=aa
```

Elasticsearchに直接ポスト

```
192.168.99.100:9200/test-doc/test/_create
```

KibanaのURL

```
192.168.99.100:5601
```

# GAからデータ取得

https://github.com/cmeerbeek/fluent-plugin-googleanalytics

