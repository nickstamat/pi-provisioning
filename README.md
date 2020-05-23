# pi-provisioning

An Ansible playbook for provisioning my Raspberry Pi with the tools I need.

## Requirements

- Ansible 2.9+

## Instructions

1.  Ensure that Pi has SSH enabled and the public key is added to _authorized_keys_.
2.  `PI_IP_ADDR=<ip>`
3.  `ansible-playbook -i "$PI_IP_ADDR," playbook.yml`
