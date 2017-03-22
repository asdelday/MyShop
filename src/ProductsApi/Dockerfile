FROM microsoft/dotnet:1.1.0-sdk-msbuild

MAINTAINER Julien Corioland, Microsoft (@jcorioland)

COPY project.json ./
COPY . /app
WORKDIR /app

ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000

RUN dotnet restore
RUN dotnet build

ENTRYPOINT ["dotnet", "run"]
