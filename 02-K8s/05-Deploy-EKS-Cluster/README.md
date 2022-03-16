# Amazon Cloud Access

## Craete a Programatic Access Key User

```
You need to a IAM User - > Login -> AWS Console -> Search (IAM) -> Create User (yourlabusername) -> Enable Progrmatic Access -> Create & Downloand Keys.

```

## Now export the AWS Keys into Env. Variables

```
echo "export AWS_ACCESS_KEY_ID="XXXXXXXXXXXX" " >> .bashrc
```

```
echo "export AWS_SECRET_ACCESS_KEY="XXXXXXYYYYYYYYYYYYYYYYYYYYYYYYYYY" " >>  .bashrc
```

```
source  .bashrc
```

```
set | grep -i AWS
```

## Download EKSCTL Binary from the following Sources: 

1. Download and extract the latest release of eksctl with the following command.

```
curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
```

2. Move the extracted binary to /usr/local/bin.
```
sudo mv /tmp/eksctl /usr/local/bin
```

3. Test that your installation was successful with the following command.
```
eksctl version
```

## Download Kubectl Binary also, if you already have the skip: 

## Let's set up EKS Cluster:

```
# eksctl create cluster --name <cluster-name> --version 1.21 --region <region> --nodegroup-name worker-nodes --node-type t2.micro --nodes 2
```

```
# eksctl create cluster --name k8s-av-user26 --version 1.21 --region us-east-2 --nodegroup-name worker-nodes --node-type t2.micro --nodes 2
```
