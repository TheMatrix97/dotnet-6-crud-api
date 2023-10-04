# dotnet-6-crud-api

.NET 6.0 - CRUD API Example

Documentation at https://jasonwatmore.com/post/2022/03/15/net-6-crud-api-example-and-tutorial

## Commands

` docker build -t testapi:latest .`

`docker run --rm -p 4000:4000 testapi:latest`

Run owasp basic api scan

`docker run -t owasp/zap2docker-weekly zap-api-scan.py -t http://host.docker.internal:4000/swagger/v1/swagger.json -f openapi`

Run owasp webui
`https://juice-shop.herokuapp.com/#/`
`docker run -u zap -p 8080:8080 -p 8090:8090 -i ghcr.io/zaproxy/zaproxy:stable zap-webswing.sh`
