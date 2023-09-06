# windows에서 쿠버네티스 사용

## virtualBox 설치
https://www.virtualbox.org/wiki/Downloads

![image](https://github.com/aamoos/kubernates/assets/37327676/d0f50eb2-4107-4eeb-a291-568b395243ce)

## minikube 설치
https://github.com/kubernetes/minikube/releases/latest/download/minikube-installer.exe

## 버전확인
minikube version

## virutal box로 minikube 실행
minikube start --driver=virtualbox

## 특정 k8s 버전 실행
minikube start --kubernetes-version=v1.25.1

## 상태확인
minikube status

## 정지
minikube stop

## 삭제
minikube delete

## ssh 접속
minikube ssh

## ip 확인
minikube ip

# 쿠버네티스에 wordpress 설치
~/Workspace/k8s/guide/index/docker-compose.yml 생성

## docker-compose 실행
- docker-compose up -d

![image](https://github.com/aamoos/kubernates/assets/37327676/a4326dd1-b08f-47d3-880b-2a8cfc9563a6)

## 워드프레스 접속
http://localhost:30000/wp-admin/install.php

![image](https://github.com/aamoos/kubernates/assets/37327676/f4864219-2492-491b-afb3-69418efddfb8)

![image](https://github.com/aamoos/kubernates/assets/37327676/dd5998e1-3b1c-4172-a0fc-2fa241706d48)

![image](https://github.com/aamoos/kubernates/assets/37327676/224f07f8-6d69-43b4-8ea1-4745e30bfe2a)

# wordpress-mysql을 쿠버네티스를 통해 설치 하기
kubectl apply -f wordpress-k8s.yml
