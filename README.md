# ubuntu24-env

ubuntu24-env for Daddy Knows Best

# history

- 01/22/2024 downgraded python version to 3.10.6
- 09/12/2024 new repo

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
07:16:47 ubuntu@d2c356fcb381 dev-env ±|main|→ cat /etc/*ease
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=24.04
DISTRIB_CODENAME=noble
DISTRIB_DESCRIPTION="Ubuntu 24.04 LTS"
PRETTY_NAME="Ubuntu 24.04 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=noble
LOGO=ubuntu-logo
07:16:53 ubuntu@d2c356fcb381 dev-env ±|main|→
```
