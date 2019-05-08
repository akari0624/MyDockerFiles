##  Dockerfiles to build the image that I use in my daily IT...

- gradle_4.10.2
  - now `alpine 3.9` (depend on ` openjdk:8-jdk-alpine:latest`)
  - jdk 8
  - suit for old JAVA environment, because `Gradle 5` start to not support to produce `JAVA 5` bytecode
  - will be `root` when in container (in order to `apk add ..dependencies`)
  - `openssh`, `sshpass`, `bash`, `sudo` pre-installed.(`apline` did not have these dependencies)
  - I take the reference from [offical gradle image docker file](https://github.com/keeganwitt/docker-gradle/blob/master/jdk8-alpine/Dockerfile) to write this my own
  - I have been use it in CI/CD pipeline in my java-library developing.
  - [docker-hub url](https://hub.docker.com/r/morris0987/gradle4.10.2)