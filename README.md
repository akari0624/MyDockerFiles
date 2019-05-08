##  Dockerfiles to build the image that I use in my daily IT...

- gradle_4.10.2
  - now `alpine 3.9`
  - jdk 8
  - suit for old JAVA environment, because `Gradle 5` start to not support to produce `JAVA 5` bytecode
  - will be `root` when in container (in order to `apk add ..dependencies`)
  - `openssh`, `sshpass`, `bash`, `sudo` pre-installed.(`apline` did not have these dependencies)
  - [docker-hub url](https://hub.docker.com/r/morris0987/gradle4.10.2)