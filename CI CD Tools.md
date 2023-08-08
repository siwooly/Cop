# CI/CD Tools

CI/CD: 개념
날짜: 2023년 8월 8일
태그: CI/CD

# Jenkins

제일 많이 사용하는 CI/CD 툴

# Tekton

클라우드 네이티브 CI/CD 시스템이다. 특히, 쿠버네티스 기반 오픈소스 프레임워크로 **기존 쿠버네티스 환경에 특화됨.** 

- **Tekton Pipeline : Takton의 기초이자 핵심 컴포넌트. 쿠버네티스의 Custom Resources로 이루어져 쿠버네티스 오브젝트로  CI/CD 파이프라인을 조립할 수 있는 빌딩 블록을 제공.**
- Tekton Dashboard
- Tekton Triggers
- Tekton CLI
- Tektion Hub

### Jenkins / Tekton / GitHub Actions 특징

> [https://velog.io/@sgwon1996/Jenkins-vs-GitHub-Action-vs-Tekton](https://velog.io/@sgwon1996/Jenkins-vs-GitHub-Action-vs-Tekton)
> 

---

---

# AgroCD

쿠버네티스 어플리케이션의 자동 배포를 위한 오픈소스 도구. Git과 쿠버네티스를 동기화 해주는 에이전트와 같은 역할을 수행. Git 기반의 변경점을 쿠버네티스에 배포하는 경우에 유용한 툴!

- CI/CD 파이프라인에서 CD 부분을 담당!

---

---

# Chef

puppet과 같이 rubyt 작성. Continuous Delivery 를 위한 솔루션.

# Puppet

ruby로 만들어진 시스템 자동화 툴. 반복되는 업무를 자동화하기 위함.

주로 설정, 관리, 배포, orchestrate와 같은 일을 하기 위해 사용.

- 관리 대상 서버에 agent 설치 필요함.
- Master서버는 Linux 서버에 설치 되어야 함.
- Agent 서버는 Linux, Windows, Solaris 등 대부분의 OS 지원.
- 8140 포트 사용
- 선언적 프로그래밍 지원함.

# Ansible

Ansible또한 Puppet과 동일한 역할을 수행한다. ansible이 사용이 좀 더 간편한 편.

Puppet은 agent 설치가 필요하지만, Ansible은 자동화 대상에 추가적 소프트웨어를 설치하지 않아도 된다. 

- Puppet은 선언전 프로그래밍인 반면에 Ansible은 실행 단계를 일일히 정의 내려주어야 함.

### 선언적 (DSL, 도메인 특정 언어 ) VS 절차적 or 명령형

> puppet의 pp 파일로 nginx 다운로드 후, 서비스 실행
> 

[https://myjamong.tistory.com/244?category=1051876](https://myjamong.tistory.com/244?category=1051876)

> Ansible playbook으로 nginx설치 하는 yaml 파일
> 

[https://kibbomi.tistory.com/258](https://kibbomi.tistory.com/258)

차이점이 공식 문서에 잘 정리되어있다.

> [https://www.redhat.com/ko/topics/automation/understanding-ansible-vs-terraform-puppet-chef-and-salt](https://www.redhat.com/ko/topics/automation/understanding-ansible-vs-terraform-puppet-chef-and-salt)
>