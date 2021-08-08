# Terraform-Ansible-Project
- Ansible의 playbook을 통해 wordpress를 배포하고, Terraform을 통해 AWS에 인스턴스를 만들고 RDS를 구축한다.

# 기본 설치 - 리눅스 버전
```
# AWS CLlv2 설치
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
sudo apt install unzip   # 리눅스는 unzip이 안깔려 있기때문에 설치해줘야 한다.
unzip awscliv2.zip
sudo ./aws/install
aws configure            # AWS CLI 구성

# Terraform 설치
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=$(dpkg --print-architecture)] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt install terraform
```
