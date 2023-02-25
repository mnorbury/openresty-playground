# OpenResty Playground

This project serves a sample app on port `8080` for `openresty:1.13` and port `8085` `openresty:latest`.

```bash
curl -XPUT  http://localhost:8080/foo -H "Content-Type: application/octet-stream" --data-binary @./data/file-coderstool.xml
```

```bash
curl -XPUT  http://localhost:8085/foo -H "Content-Type: application/octet-stream" --data-binary @./data/file-coderstool.xml
```

The digest for the test file is `zdwNsIbtCjb0s4WvqUNgMWV2kOLoSKcvR+HsRdOB24s=`

```bash
❯ openssl dgst -sha256 -binary ./data/file-coderstool.xml | openssl enc -base64 -A
zdwNsIbtCjb0s4WvqUNgMWV2kOLoSKcvR+HsRdOB24s=
```
