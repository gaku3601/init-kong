# apiの登録
curl -i -X POST   --url http://localhost:8001/apis/   --data 'name=test' --data 'uris=/test' --data 'upstream_url=http://mockbin.org'
