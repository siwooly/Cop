# Docker, Container Orchestration, EKS Tools

CI/CD: 개념
날짜: 2023년 8월 8일
태그: CI/CD

# Docker

- **Docker compose : 단일 머신에서 여러 컨테이너 간단하게 관리하지만 swarm 보다는 가용성이 떨어짐.**
- **Docker swarm** : Container orchestartion, 클러스터링, 스케쥴링을 위한 오케스트레이션 툴. K8S로 보면 된다.

# Rancher

**쿠버네티스 운영 관리를 위한 플랫폼**

여러 클라우드 환경에서 제공되는 쿠버네티스를 쉽게 연동하여 관리, 운영 및 보안 문제를 해결!

도커 기반의 시스템으로 도커 설치 필수!

- 그라파나, 프로메테우스 등 모니터링 도구 쉽게 연동 가능
- Istio 가능

# ECS, EKS VS EC2, Fargate

> 한 줄 요약 : ECS, EKS를 동작시키기 위한 컴퓨팅 리소스가 EC2, Fargate이다.
> 

ECS, EKS 는 컨테이너 오케스트레이션이며 EC2, Fargate는 호스팅에 대한 레이어를 담당하는 제품.

# ECS VS EKS

> 둘 다 컨테이너 오케스트레이션 환경이지만, ECS는 AWS에서만 제공되는 오케스트레이션 환경으로 다른 클라우드 환경에서 이식성은 떨어지지만, EKS는 K8S 기반의 서비스이기 때문에 이식성이 좋다.
> 

# EC2 vs Fargate

> EC2는 가상화된 VM(가상머신)이지만 Fargate는 좀 더 추상화된 컴퓨팅 환경이다. EC2의 서버리스 버전이라 보면 된다.
> 

---

---

---

# Istio

service mesh 

# Helm과 Harbor

## Helm

***쿠버네티스 패키지 매니저***. python에서는 pip 툴, centOS에서는 yum 같이 패키지를 관리 해주는 툴이다. helm을 이용하면 원하는 패키지들을 쿠버네티스에 쉽게 설치할 수 있다!

## Harbor

프라이빗 레지스트리로 도커 이미지를 저장하고 분배하는 기업용 레지스트리 서버이다.

퍼블릭한 Docker Hub와 다르게 프라이빗하게 사용하도록 개인 서버에 구축하는 ***도커 이미지 저장소***

![이거를 보면 무엇인지 확 와닿는당.](Docker,%20Container%20Orchestration,%20EKS%20Tools%207ba8d4b1912745dd9783f5761137f1a4/Untitled.png)

이거를 보면 무엇인지 확 와닿는당.

#