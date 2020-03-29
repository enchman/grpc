# GRPC

## Instructions
* Create Solution.
* Add **grpc service** project.
  * If project is client, than add GRPC.Tools from nuget package to the project.
* Add .proto file in **/Protos**
* Add Protobuf to .csproj if project is client replace value in GrpcServices="Server" to "Client"
``` 
  <ItemGroup> 
    <Protobuf Include="Protos\<filename>.proto" GrpcServices="Server" />
  </ItemGroup>
```
* This will generate code for .proto
