# 初期設定

    docker-compose up -d
    dc run kong kong migrations up

その後再起動

# apiの登録
curl -i -X POST   --url http://localhost:8001/apis/   --data 'name=test' --data 'uris=/test' --data 'upstream_url=http://mockbin.org'
