# Deploy a .NET Core API with Docker

## From
- Les Jackson https://www.youtube.com/watch?v=f0lMGPB10bM&t=3s

### Overview
- .NET 5
- Docker

#### .Net 5 commands
- dotnet --version
- dotnet new webapi -n {name}
- dotnet build
- dotnet run

#### Docker help
- Dockerize an ASP.NET Core application https://docs.docker.com/samples/dotnetcore/
- docker --version
- Build an image: docker build -t {your docker hub id}/{image name} . --> julianecheverri23/platformservice (dont forget the period!)
- For running an image as a container: docker run -p 8080:80 -d {your docker hub id}/{image name} --> julianecheverri23/platformservice
- For seeing containers running: docker ps
- For stop container: docker stop {CONTAINER ID}
- For start a container: docker start {CONTAINER ID}
- For publish container: docker push {your docker hub id}/{image name}
- Running service url http://localhost:8080/api/platforms/
- docker login -u "myusername" -p "mypassword" docker.io