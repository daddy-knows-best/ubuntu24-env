# ubuntu24-env

ubuntu24-env for Daddy Knows Best

# history

01/22/2024 downgraded python version to 3.10.6
09/12/2024 new repo

# installed packages

- pyenv
- pipenv
- ansible
- pre-commit
- detect-secrets (Yelp)
- docker in docker, kubectl
- github action: pre-commit, docker-publish

# how to run

```
$ docker compose pull
[+] Pulling 14/14
 ✔ dev-env 13 layers [⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿]      0B/0B      Pulled                                        225.6s
   ✔ 445a6a12be2b Already exists                                                                     0.0s
   ✔ 5e8cb166128c Already exists                                                                     0.0s
   ✔ 1f4f7116f9c7 Already exists                                                                     0.0s
   ✔ 89bc601657a4 Pull complete                                                                    136.5s
   ✔ d2964040b138 Pull complete                                                                    136.7s
   ✔ 58ee2e35305f Pull complete                                                                    136.8s
   ✔ ff7916016ca2 Pull complete                                                                    152.8s
   ✔ a137eb12f207 Pull complete                                                                    202.9s
   ✔ f0c43ee4ac0a Pull complete                                                                    203.5s
   ✔ 93093980a774 Pull complete                                                                    205.3s
   ✔ 706010b009a5 Pull complete                                                                    223.1s
   ✔ c54d94ba6b3c Pull complete                                                                    223.3s
   ✔ 5ac553ae35ad Pull complete                                                                    223.4s

$ docker compose run --rm dev-env
03:06:30 ubuntu@3ae73b23d384 dev-env ±|main|→ ls
Dockerfile  LICENSE  README.md  docker-compose.yaml
03:06:33 ubuntu@3ae73b23d384 dev-env ±|main|→
03:28:53 ubuntu@78e06ea681cd dev-env ±|main|→ pyenv versions
  system
* 3.11.5 (set by /home/ubuntu/.pyenv/version)
03:29:01 ubuntu@78e06ea681cd dev-env ±|main|→ ansible --version
ansible [core 2.15.4]
  config file = None
  configured module search path = ['/home/ubuntu/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /home/ubuntu/.pyenv/versions/3.11.5/lib/python3.11/site-packages/ansible
  ansible collection location = /home/ubuntu/.ansible/collections:/usr/share/ansible/collections
  executable location = /home/ubuntu/.pyenv/versions/3.11.5/bin/ansible
  python version = 3.11.5 (main, Sep 16 2023, 18:50:11) [GCC 11.4.0] (/home/ubuntu/.pyenv/versions/3.11.5/bin/python3.11)
  jinja version = 3.1.2
  libyaml = True
03:29:05 ubuntu@78e06ea681cd dev-env ±|main|→
```
