FROM microsoft/dotnet:latest

MAINTAINER Julien Corioland, Microsoft (@jcorioland)

COPY project.json ./
COPY . /app
WORKDIR /app

ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000


RUN dotnet restore
RUN dotnet build

ENTRYPOINT ["dotnet", "run"]
