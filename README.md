# GRpc Spring Boot Starter

## Usage

* Add dependencies (see examples)

```
io.grpc:grpc-stub
io.grpc:grpc-protobuf
io.grpc:grpc-netty
```    
    
* Add `@EnableGRpcServer` anotation to your configuration for enable grpc server
* Customize configuration - application.yml/application.property. Example:

```YAML
grpc:
 enabled: true
 servers:
   -
     address: 127.0.0.1
     port: 6565
   -
     address: 127.0.0.1
     port: 6566
```

or

```ini  
    grpc.enabled: true
    grpc.servers[0].address=127.0.0.1
    grpc.servers[0].port=6565
```    

## Default values

* port 6565
* host/ip localhost/127.0.0.1

## Tested on

| name                      | version       |
| ---                       | ---           |
| io.grpc:grpc-stub         | 0.13.1        |
| io.grpc:grpc-protobuf     | 0.13.1        |
| io.grpc:grpc-netty        | 0.13.1        |
| com.google.protobufprotoc | 3.0.0-beta-2  |
| Spring Boot               | 1.3.3.RELEASE |
