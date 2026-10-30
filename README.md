# :trophy: CKA Exam prep

Learn kubernetes they said ... It would be fun they said ...

## :books: The back story

I wanted to learn more about k8s since we were using it at work. Naive me, thought the CKA Exam would be the best way to do this since there would know everything there is. Why not take the CKAD exam you wonder? Well ... who takes the CKAD exam, that sounds like the noob exam. I am smart I need a real challenge. I will do the CKA exam. 2 years and 2 failed attemps later, here we are creating yet another repository to try and pass the exam, because it would be a waste to let the already company spent learning and development budget go down the drain. And yes, you read correctly... I bought yet another exam attempt. 2 failures were not enough for me to give up. So as you see I've gotten myself into this mess. Let's see what we can make of it. 

## Setup

1. Setup a google cloud project with billing attached

2. This repo uses [mise](https://mise.jdx.dev/installing-mise.html#mise-run). You can install the dependencies via `mise install` and activate the mise environment via `mise en`.

```bash
mise install    # install the dependencies
mise en         # activate the env
```

3. Initaliaze gcloud to connect to your google project

```bash 
gcloud init                             # connect to your google project
gcloud auth application-default login   # authenticate for terraform
```

## Terraform

Install the infrastructure.

```bash
cd terraform
terraform plan      
terraform apply
```

Destroy the infrstructure

```bash
terraform destroy
```

# Developer

```bash
terraform fmt -recursive
```