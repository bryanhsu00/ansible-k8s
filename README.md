# ansible-k8s

## Introduction
Use ansible to create an k8s cluster with single master nodes and three worker nodes automatically.

## Environment
- ubuntu 20.04
- kubeadm 1.22
- CRI: cri-o 19.03
- CNI: flannel

## Prerequisite
Edit `inventory/hosts` and `group_vars/all.yaml` as your desired

## Usage
- build - `ansible-playbook site.yaml -i inventory/hosts`
- cleanup - `ansible-playbook reset-site.yaml -i inventory/hosts`
