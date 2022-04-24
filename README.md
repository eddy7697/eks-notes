# eks-notes
EKS 筆記

## Install aws cli

```
$ sudo apt update
$ pip install awscli
```

## 2. Install kubectl: for linux
```
$ curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
$ chmod +x ./kubectl
$ mv ./kubectl /usr/local/bin/kubectl
$ kubectl version --short --client
```

## 3. Install aws-iam-authenticator
###  see: https://docs.aws.amazon.com/zh_tw/eks/latest/userguide/install-aws-iam-authenticator.html
```
$ curl -o aws-iam-authenticator.sha256 https://amazon-eks.s3.us-west-2.amazonaws.com/1.21.2/2021-07-05/bin/linux/amd64/aws-iam-authenticator.sha256
$ chmod +x ./aws-iam-authenticator
$ sudo mv aws-iam-authenticator /usr/local/bin
$ aws-iam-authenticator version --short
```

## VPC consideration