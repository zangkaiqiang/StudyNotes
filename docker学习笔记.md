### docker run 
docker run -it --rm images bash

### docker commit

docker commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]

OPTIONS:

|Name| shorthand|	Default|	Description|
|-----|--------|-------|-------|
|--author | -a	||	Author (e.g., “John Hannibal Smith hannibal@a-team.com”)|
|--change| -c		||Apply Dockerfile instruction to the created image|
|--message | -m	|	|Commit message|
|--pause | -p	|true	|Pause container during commit|

EXAMPLE:

docker commit -m "update" container_id zangkaiqiang/commit_test:v2

### 删除所有容器
docker rm `docker ps -a -q`

### 删除所有镜像
docker rmi `docker images -q`

### 删除已经退出的容器
docker rm `docker ps -a| grep Exited | awk '{print $1}'`

### 强制删除镜像
docker rmi --force imageid|imagerepository

### 强制删除容器
docker rm -f container
