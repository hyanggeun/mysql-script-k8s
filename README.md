# Mysql in K8S

* k8s환경에서 1 master 1 slave 구조를 테스트 하기 위해 만든 yaml
* mysql Version: ```5.7.31```
### 디렉토리 구조

    mysql
    ㄴ master-cm.yaml
    ㄴ master-sts.yaml
    ㄴ service.yaml
    ㄴ slave-cm.yaml
    ㄴ slave-sts.yaml
    
### 사용법
```bash
cd ./mysql-yaml
kubectl apply -f .
```
* my.cnf 설정을 바꾸고 싶다면
    * ```master-cm.yaml```, ```slave-cm.yaml```에서 변경하고 ```kubectl apply``` 를 다시 해주면 된다. 