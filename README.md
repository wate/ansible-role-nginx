nginx
=================

setup Nginx web server

OS Platform
-----------------

### Debian

- bullseye
- buster

Role Variables
--------------

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードを参照してください。

### `nginx_packages`

インストールするパッケージ

### `nginx_default_client_max_body_size`

アップロードサイズの上限

### `nginx_vhosts`

バーチャルホストの設定

### `nginx_generate_dh_key`

Diffie–Hellmanキーを生成するか否か

### `nginx_dh_key_bit`

Diffie–Hellmanキーのビット数

### `nginx_dh_key_path`

Diffie–Hellmanキーのパス

### `nginx_cfg_ssl_protocols`

SSL/TLSバージョンの設定

### `nginx_cfg_ssl_ciphers`

SSL Cipherの設定

### `nginx_cfg`

Nginxの全体設定

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: nginx
```

License
--------------

Apache License 2.0
