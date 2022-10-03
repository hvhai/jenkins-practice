# Jenkins tutorial

## Run jenkin from docker

```shell
docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```

## Create multiple branches pipeline

1. Create credential

    Credential scope:
    - global: Everywhere
    - system: Only for Jenkins server not for Jenkins job
    - project: Only for the project pipeline

2. Add credential to the project config
   ![config branch](docs/assets/config-branch-sources.png)
3. Run scan source in pipline
   ![run scan source](docs/assets/run-scan-pipeline.png)

