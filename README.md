# Git Flow
---

## Instalar Git flow
- sudo apt install git-flow

## Verificar versão
- git flow version

## Comandos
- Iniciar o git flow
  - git flow init ou git flow init -f para forçar inicialização
  - alem da master tem que criar a branch develop
  - comando:
        - git branch develop
  - Criado o develop devemos iniciar com
- Devemos iniciar a feature.
Comando:
  - git flow feature start _nome_da_feature
Para finalizar a feature executar o comando:
  - git flow feature finish _nome_da_feature

OBS.: criar feature para cada modulo do desenvolvimento, ao finalizar um modulo finalizar a feature e então teremos o processo de homologação em develop, ao finalizar a feature mudamos automaticamente para develop

- Para visualizar o nome da feature execute o comando:
git branch -> mostrará o nome da feature que estamos conectado.

- Após realizar todos os teste na deve e projeto esta ok, devemos gerar a release.
- acessar o branck marter e criar a release.
Comandos:
git checkout marter
git flow release start 1.0.0
OBS.: ao criar a release estando na master iremos mudar para release direto e a realise será criada baseandos na develop

- podemos verifiar com git status e se tiver tudo ok podemos finalizar a release com comando:
git flow release finish _version_da_release

corrigir 
sudo dpkg --configure -a