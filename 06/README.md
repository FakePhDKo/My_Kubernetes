# Kubernetes 클러스터 핵심 개념 실습 📚
## 📖 프로젝트 개요
이 디렉터리는 쿠버네티스 클러스터의 핵심 오브젝트들을 실습하며 학습한 결과물입니다. **Pod, Deployment, Service**와 같은 기본적인 배포 단위부터, **Volume, Secret, NetworkPolicy**에 이르기까지 쿠버네티스 관리자에게 필요한 핵심 개념들을 체계적으로 다룹니다.

모든 실습은 YAML 매니페스트 파일을 작성하고 kubectl 명령어를 사용해 클러스터에서 직접 실행하는 방식으로 진행되었습니다.

## 🚀 주요 학습 내용
+ 기본 배포 단위: Pod, Deployment, ReplicaSet의 역할을 이해하고 YAML 매니페스트 파일을 작성했습니다.

+ 네트워킹: Service를 사용해 Pod를 노출하고, NetworkPolicy로 Pod 간 통신을 제어하는 방법을 익혔습니다.

+ 스토리지: PersistentVolume과 PersistentVolumeClaim을 사용해 데이터를 영구적으로 보존하는 방법을 실습했습니다.

+ 보안 및 설정: Secret과 ConfigMap으로 민감한 데이터와 설정을 안전하게 관리하는 방법을 배웠습니다.

+ 가용성: Liveness 및 Readiness Probe를 설정하여 컨테이너의 상태를 확인하고, 애플리케이션의 안정성을 높이는 방법을 익혔습니다.

##📂 프로젝트 디렉터리
+ cj: CronJob 예시 실습.

+ deploy: nginx로 서버를 구성하고 replicas 설정을 테스트하는 Deployment.

+ ds: DaemonSet 예시 실습.

+ job: CentOS 7버전 컨테이너 내부의 쉘에 명령어를 전달하여 job 실습.

+ rc: Replication Controller 실습.

+ rs: ReplicaSet 실습.

+ sts: StatefulSet 실습.

+ labs: Deployment 실습.

## 🛠️ 실행 방법
각 서브 디렉터리로 이동하여 매니페스트 파일(.yml)을 확인하고, 아래 명령어를 통해 직접 클러스터에서 실습을 진행해 볼 수 있습니다.

Bash

### 매니페스트 파일 적용
```bash
kubectl apply -f [파일명.yml]
```
### 배포된 리소스 확인
```bash
kubectl get pods
```

### 리소스 삭제
```bash
kubectl delete -f [파일명.yml]
```
