

# 下载golang: golang.org/dl/

# 配置国内镜像: https://github.com/goproxy/goproxy.cn

```
go env -w GO111MODULE=on
go env -w GOPROXY=https://goproxy.cn,direct

#获取使用aliyun
go env -w GOPROXY=https://mirrors.aliyun.com/goproxy/
```

# gRPC

```
https://github.com/grpc/grpc-go

#installation
$ go get -u google.golang.org/grpc

```

# Protoc: protobuf编译器，将.proto文件转译成protobuf的原生数据结构

```
#protoc:
https://github.com/protocolbuffers/protobuf/releases

#protoc sample usage:

$ protoc --go_out=plugins=grpc:. <proto-file-name>.proto

$ protoc --proto_path=proto/hello.proto --go_out=plugins=grpc:servies proto/hello.proto

#proto3 doc:
https://developers.google.com/protocol-buffers/docs/gotutorial

#protobuf:
https://github.com/protocolbuffers/protobuf

#golang library:
https://github.com/golang/protobuf

```

# protoc-gen-go： 在GOPATH的bin目录下生成可执行文件.protobuf的编译器插件protoc-gen-go
执行protoc命令时会自动调用该插件

```
#installation
go get https://github.com/golang/protobuf/protoc-gen-go
```