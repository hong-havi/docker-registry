# docker-registry
Docker Registry

## 준비과정
### 아래의 폴더 생성
./data
./log

### secrets 설정
./secrets/ssl/~~

## Build & Up
```
$ docker-compose -f docker-compose.yml up -d --build
```


## 명령어
- 아래의 curl을 cli 에서 조회하거나 도메인 설정이 되어 있을시 도메인으로 조회
- 기본 로컬 domain 은 localhost 조회
### Repositories Search
```
$ curl -X GET http://{domain}/v2/_catalog
```
### Repositories Tag List
```
$ curl -X GET http://{domain}/v2/{repository name}/tags/list
```

###
