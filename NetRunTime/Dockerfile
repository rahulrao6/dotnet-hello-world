FROM mcr.microsoft.com/dotnet/runtime:latest
WORKDIR /app
COPY bin/Release/net7.0/publish/ .
ENTRYPOINT ["dotnet", "HelloWorld.dll"]
