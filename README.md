# controller-casc-examples
Repository designed to store controller objects using Configuration as Code principles

To apply any configuration, just run the following command:

```console
ansible-navigator run playbooks/config-controller.yaml -i localhost -m stdout --eei quay.io/automationiberia/casc/ee-casc:latest --vault-password-file .vault-password -e @vars/vault.yaml -e @vars/paths-controller.yaml -e@vars/vault-controller_iam.yaml --vault-password-file .vault-password -e '{controller_configuration_filetree_read_secure_logging: false,ansible_async_dir: /home/runner/.ansible_async/}'
```
