# wallaby

Yalk Flutter project

## How to run?

- Install Flutter
  - See https://flutter.dev/docs/get-started/install
- Install protobuf & protoc plugin for dart
  - See https://grpc.io/docs/quickstart/dart/
- Compile proto files at root of project
  - `mkdir -p lib/generated; protoc --dart_out=grpc:lib/generated -Iproto proto/*`
- Run flutter app
  - `flutter run [-d <device id>]`
  - If device is chrome, gRPC will not work without proxy

## TODO

- [ ] Extract channel to hide different native/web channel implementation
- [ ] Configure channel address with environment
- [ ] Extract proto as git submodule
