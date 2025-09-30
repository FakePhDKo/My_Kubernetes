# 📂 07(서비스(Service))
이 디렉토리는 쿠버네티스 서비스의 핵심 개념을 실습하고 이해하는 데 중점을 둡니다. 파드에 대한 안정적인 접근점을 제공하고, 외부 트래픽을 파드로 분산하는 다양한 서비스 타입을 다룹니다.

## 📌 주요 학습 내용
+ ClusterIP 서비스: 클러스터 내부 통신에 사용되는 기본 서비스 타입을 실습합니다.

+ NodePort 서비스: 모든 노드의 특정 포트를 통해 외부에서 서비스에 접근하는 방법을 배웁니다.

+ LoadBalancer 서비스: 클라우드 제공자의 로드 밸런서를 활용하여 외부 트래픽을 처리하는 방법을 익힙니다.

+ Headless 서비스: DNS를 통해 각 파드에 직접 접근해야 하는 고급 시나리오를 실습합니다.

+ ExternalName 서비스: 외부 서비스를 쿠버네티스 내부에서 별칭으로 사용하는 방법을 익힙니다.

## 📂 파일 구조

```
07/
├── headless/
│   └── headless-nginx.yml
└── svc/
    ├── externalname.yml
    ├── ip.sh
    ├── ip.txt
    ├── nginx-clusterip-svc.yml
    ├── nginx-deploy.yml
    ├── nginx-loadbalancer-svc.yml
    ├── nginx-loadbalancer-svc2.yml
    ├── nginx-nodeport-svc.yml
    ├── server.list
    └── test-svc.yml
```
## 📝 디렉토리 설명
+ headless/: 헤드리스 서비스 관련 파일을 포함합니다.

+ headless-nginx.yml: ClusterIP: None을 명시하여 로드 밸런싱 없이 각 파드의 DNS 레코드를 생성하는 헤드리스 서비스를 정의합니다.

+ svc/: 다양한 유형의 서비스를 다룹니다.

+ nginx-deploy.yml: Nginx 파드들을 생성하는 Deployment 매니페스트입니다.

+ nginx-clusterip-svc.yml: ClusterIP 타입의 서비스를 생성합니다.

+ nginx-nodeport-svc.yml: NodePort 타입의 서비스를 생성합니다.

+ nginx-loadbalancer-svc.yml, nginx-loadbalancer-svc2.yml: LoadBalancer 타입의 서비스를 생성하는 예제입니다.

+ externalname.yml: 외부 도메인에 대한 별칭을 만드는 ExternalName 서비스를 정의합니다.

+ ip.sh, ip.txt, server.list: 파드 IP 주소 확인 및 서버 목록 관리를 위한 스크립트 및 파일입니다.

+ test-svc.yml: 클러스터IP 테스트 파일입니다.
