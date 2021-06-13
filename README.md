# ansible-k8s

## Introduction
Use ansible to create an HA k8s cluster with three master nodes and three worker nodes automatically.

## Environment
- ubuntu 18.04
- kubeadm 1.20
- CRI: docker 19.03
- CNI: calico

## Prerequisite
Edit `inventory/hosts` and `group_vars/all.yaml` as your desired

## Usage
- build - `ansible-playbook site.yaml -i inventory/hosts`
- cleanup - `ansible-playbook reset-site.yaml -i inventory/hosts`