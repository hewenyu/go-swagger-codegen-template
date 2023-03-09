# go-swagger-codegen-template
swagger-codegen 的 go 代码模板更新 自用



```bash
# Download current stable 2.x.x branch (Swagger and OpenAPI version 2)
wget https://repo1.maven.org/maven2/io/swagger/swagger-codegen-cli/2.4.30/swagger-codegen-cli-2.4.30.jar -O swagger-codegen-cli.jar

java -jar swagger-codegen-cli.jar help

# Download current stable 3.x.x branch (OpenAPI version 3)
wget https://repo1.maven.org/maven2/io/swagger/codegen/v3/swagger-codegen-cli/3.0.41/swagger-codegen-cli-3.0.41.jar -O swagger-codegen-cli.jar

java -jar swagger-codegen-cli.jar --help
```


# Example Usage
```console
# git clone 
git clone https://github.com/hewenyu/go-swagger-codegen-template.git && cd go-swagger-codegen-template
```


```console
# use client
# env java 8 +

# 生成sdk
java -jar swagger-codegen-cli.jar generate -i https://petstore.swagger.io/v2/swagger.json -l go -o /go/

# 生成 server
java -jar swagger-codegen-cli.jar generate -i https://petstore.swagger.io/v2/swagger.json -l go-server -o /go-server/
```

