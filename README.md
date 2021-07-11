# pi-provisioning

An Ansible playbook for provisioning my Raspberry Pi fleet with k3s.

This is based on https://github.com/k3s-io/k3s-ansible, but I've stripped out all Raspbian-/CentOS-related parts which are not relevant for my own setup, for the sake of simplicity.

## Instructions

Create and adjust inventory:

```
cp -R inventory/sample inventory/my-cluster
```

Start provisioning:

```
ansible-playbook site.yml -i inventory/my-cluster/hosts.ini
```
