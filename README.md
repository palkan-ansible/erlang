Erlang
========

Installs Erlang.

Installation
--------------

`ansible-galaxy install palkan.erlang`

Role Variables
--------------

`defaults/main.yml`

| Name                        | Default Value |  Description    |
|-----------------------------|---------------|-----------------|
| erlang_version              | "17.5"        | Erlang version to install |
| erlang_check_version        | "17.5"        | Version name to checke if already installed |
| erlang_url                  | "http://www.erlang.org/download/otp_src_{{ erlang_version }}.tar.gz" | Source tar url | 
| erlang_name                 | "otp_src_{{ erlang_version }}" | |
| erlang_tmp_path             | "/usr/local/src/{{ erlang_name }}" | Where to download source | 


Example Playbook
-------------------------
```yml
  - hosts: servers
    roles:
       - palkan.erlang
```
