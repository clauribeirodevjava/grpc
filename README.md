# grpc

## Em quais casos podemos usar?
###
- Ideal para microserviços
- Mobile, Browsers e Backend
- Geração das bibliotecas de forma automática
- Steraming bidirecional utilizando HTTP/2

  # Linguagens (Suporte oficial)
  - gRPC-GO
  - gRPC-JAVA
  - gRPC-C
      - C++
      - Python
      - ...etc

  
  **RPC ilustração**

![](image/clientserver.png)

# Instalação
## protobuf
```
sudo apt-get install -y protobuf-compiler

protoc --version
```

# Gerar os stubs para o gRPC

protoc --go_out=. --go-grpc_out=. proto/course_category.proto

#Copiar os datasources do projeto graphQL

#Criar os protos 
```

syntax = "proto3";
package pb;
option go_package = "internal/pb";

message Category {
    string id = 1;
    string nome = 2;
    string description = 3;
}
message CreateCategoryRequest{
    string name = 1;
    string description = 2;
}
message CategoryResponse {
    Category category = 1;
}

service CategoryService {
    rpc CreateCategory(CreateCategoryRequest) returns (CategoryResponse){}
}

```

#Rodar o comando para gerar os stubs:
```
protoc --go_out=. --go-grpc_out=. proto/course_category.proto
```
#Vai gerar os stubs 







# Como Usar
Aqui estão as instruções sobre como usar o meu aplicativo.

- [ ] [https://github.com/clauribeirodevjava/grpc/issues/1#issue-1967380355)](https://github.com/clauribeirodevjava/grpc/issues/1#issue-1967380355)
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
