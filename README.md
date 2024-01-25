[![SCA](https://github.com/stiifii/tbo_projekt/actions/workflows/dependency_check.yml/badge.svg)](https://github.com/stiifii/tbo_projekt/actions/workflows/dependency_check.yml)
[![SAST](https://github.com/stiifii/tbo_projekt/actions/workflows/bandit.yml/badge.svg)](https://github.com/stiifii/tbo_projekt/actions/workflows/bandit.yml)
[![Python Unit Tests](https://github.com/stiifii/tbo_projekt/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/stiifii/tbo_projekt/actions/workflows/unit-tests.yml)
[![DAST](https://github.com/stiifii/tbo_projekt/actions/workflows/zap.yml/badge.svg)](https://github.com/stiifii/tbo_projekt/actions/workflows/zap.yml)
# TBO - Projekt
Autorzy: 
- Michał Adrjan
- Hubert Decyusz
- Daniel Stefański
## CICD
Do stowrzenia CICD przy użyciu GitHub Actions zostały użyte narzędzia:
- SAST - [Bandit](https://github.com/PyCQA/bandit)
- DAST - [ZAProxy](https://github.com/zaproxy/zaproxy)
- SCA - [Dependency Check](https://github.com/jeremylong/DependencyCheck)

## Komponenty
- [Workflow dla budowy obrazu z gałęzi main z tagiem: latest](.gitub/workflows/main-build-and-push.yml)
- [Workflow dla budowy obrazu z innej gałęzi z tagiem: beta](.gitub/workflows/build-and-push.yml)
- [Workflow do uruchomienia SAST Bandit](.gitub/workflows/bandit.yml)
- [Workflow do uruchomienia ZAP](.gitub/workflows/zap.yml)
- [Workflow do uruchomienia Dependency Check](.gitub/workflows/dependency_check.yml)
- [DockerHUB repo](https://hub.docker.com/r/stiifii/tbo_projekt)

- [Workflow do wykonania testów jednostkowych](.gitub/workflows/unit-tests.yml)
## Zadanie 1
- [X] Gdy nastąpi PUSH do gałęzi main tworzy się nowy image w DockerHub z tagiem latest.
- [X] SCA, SAST oraz DAST zostają uruchomione, gdy zostaje stworzony Pull Request do gałęzi main

## Zadanie 2
Weryfikacja procesu CICD.
