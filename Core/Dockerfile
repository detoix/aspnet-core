FROM microsoft/aspnetcore
WORKDIR /app
COPY ./publish .
CMD ASPNETCORE_URLS=http://*:$PORT dotnet aspnet-core.dll
