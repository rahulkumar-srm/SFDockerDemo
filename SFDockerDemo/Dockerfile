# Ensure the Service Fabric cluster you deploy to supports the container image you are using. See https://aka.ms/containerimagehelp for information on Windows container version compatibility.
FROM microsoft/dotnet:2.2-sdk-nanoserver-1809 AS build
ARG source
WORKDIR /app
COPY ${source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "SFDockerDemo.dll"]
