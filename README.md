# Protobuf_Unity

Forked from Google Protobuf, optimized and compiled for Unity.

### Compiling Steps
1. Open with VS2022: `csharp/src/Google.Protobuf.sln`
2. Ensure there is NO `net50` in `TargetFrameworks` in `csharp/src/Google.Protobuf/Google.Protobuf.csproj`
3. Run `dotnet --list-sdks` in cmd, get the dotnet sdk version
4. Modify the `version` field in `global.json` with the dotnet sdk version
5. Switch VS to `Release` mode and build
6. The DLLs is generated in `csharp/src/Google.Protobuf/bin/Release/net45`
7. Copy the DLLs to `Plugins` folder of Unity


[Download](https://github.com/protocolbuffers/protobuf/releases) the same version protoc to compile proto message
