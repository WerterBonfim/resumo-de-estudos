

## Montando um micro container from Scratch com Rust
https://www.youtube.com/watch?v=uTUHRIMkdxw

### ferramentas
    - docker-slim


### Otimização de container aspnet
https://youtu.be/uTUHRIMkdxw?t=4826

```Dockerfile
FROM mcr.microsoft.com/dotnet/runtime-deps:6.0-alpine as base
FROM mcr.microsoft.com/dotnet/sdk:6.0 as build

RUN dotnet publish projeto.csproj --self-contained -c Release -r linux-musl-x64 -p:publishTrimmed=true -o /app/publish
```
