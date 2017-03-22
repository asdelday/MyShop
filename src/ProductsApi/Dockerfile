FROM microsoft/dotnet:1.1.0-sdk-msbuild

MAINTAINER Julien Corioland, Microsoft (@jcorioland)

COPY . /app
WORKDIR /app

ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000

RUN ["dotnet", "restore", "/app"]
RUN dotnet build /app

ENTRYPOINT ["dotnet", "run"]
