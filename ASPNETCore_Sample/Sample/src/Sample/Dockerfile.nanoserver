FROM microsoft/dotnet:nanoserver
ENTRYPOINT ["dotnet", "Sample.dll"]
ARG source=.
WORKDIR /app
ENV ASPNETCORE_URLS http://+:82
EXPOSE 82
COPY $source .