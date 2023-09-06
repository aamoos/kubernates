# windows에서 쿠버네티스 사용

# virtualBox 설치
https://www.virtualbox.org/wiki/Downloads

![image](https://github.com/aamoos/kubernates/assets/37327676/d0f50eb2-4107-4eeb-a291-568b395243ce)

# minikube 설치
https://github.com/kubernetes/minikube/releases/latest/download/minikube-installer.exe

# 버전확인
minikube version

# virutal box로 minikube 실행
minikube start --driver=virtualbox

# 특정 k8s 버전 실행
minikube start --kubernetes-version=v1.23.1

# 상태확인
minikube status

# 정지
minikube stop

# 삭제
minikube delete

# ssh 접속
minikube ssh

# ip 확인
minikube ip
