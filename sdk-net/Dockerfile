FROM mcr.microsoft.com/dotnet/sdk:7.0
WORKDIR /app
COPY bin/Release/net7.0/publish/ .
ENTRYPOINT ["dotnet", "HelloWorld.dll"]
