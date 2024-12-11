# SampleApp-SonarQube

1. Run docker

```sh
docker run -it --rm mcr.microsoft.com/dotnet/sdk:latest bash
```

2. Clone git repo

```sh
git clone -b dotnet https://github.com/mothkim/workout-lifebalance.git
```


```sh
dotnet tool install --global dotnet-sonarscanner
dotnet sonarscanner begin /k:"project-key" /d:sonar.login=admin /d:sonar.password=admin
dotnet build <path_to_solution.sln>
dotnet sonarscanner end /d:sonar.login=admin /d:sonar.password=admin
```
