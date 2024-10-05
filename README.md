nginx
=================

setup Nginx web server

OS Platform
-----------------

### Debian

- bookworm
- bullseye

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `nginx_packages`

インストールするパッケージ

#### `nginx_append_goaccess_repository`

goaccessリポジトリを追加するか否か

#### `nginx_default_client_max_body_size`

アップロードサイズの上限

#### `nginx_vhosts`

バーチャルホストの設定

#### `nginx_generate_dh_key`

Diffie–Hellmanキーを生成するか否か

#### `nginx_dh_key_bit`

Diffie–Hellmanキーのビット数

#### `nginx_dh_key_path`

Diffie–Hellmanキーのパス

#### `nginx_cfg_ssl_protocols`

SSL/TLSバージョンの設定

#### `nginx_cfg_ssl_ciphers`

SSL Cipherの設定

#### `nginx_cfg`

Nginxの全体設定

#### `nginx_modsecurity_include_files`

ModSecurityを有効にする場合に読み込むルールファイル

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `nginx_goaccess_apt_key_url`

#### `nginx_goaccess_apt_key_download_dest`

#### `nginx_goaccess_apt_key_dest`

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
