# ansible-nginx

Playbook for deploying nginx on AmazonLinux2.

### Install ansible

```sh
pip install ansible

ansible --version
  # ansible 2.9.10
  # ...
```

### Create SSH-Key

```sh
ssh-keygen -t rsa
```

作成した鍵の公開鍵をデプロイ先のホストに設定


### Create hosts file

```sh
cat <<EOT > hosts
# Destination host name or IP address.
...
EOT
```

### Deployment

```sh
ansible-playbook -v -i hosts site.yml
```
